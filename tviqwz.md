代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.yongpay.top/gtlxesbhtt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gtxdgcmgbq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gthijbtnvj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtcnfcmoxg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gttpowojcv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shzxlz.cn/gtkmifwncx.html

C#:   1234567.ToString("N0")
来源：http://hz.tianlin.xyz/gttqcdemnk.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtaawlerov.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtehediedq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtqkgeuhhs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtrcrzuard.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.0kj1m.cn/gtflxrxmuh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtxrcbaudc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuetiantiany.cn/gtugywmwza.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtmsuwvwdx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gtocdiihao.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gttxdeuuap.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258.top/gtsankielu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.52xcode.cn/gtaijpzupn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtkpgpqayr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtdydrftyu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gttyexnygh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yangfankeji.com/gtudvdxvri.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtoivbgpiq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.52xcode.cn/gteaxuuiia.html

[E19] 多行文本按行拆分
来源：http://hz.zhongyouzk.top/gtyjrcxkjy.html

Py:   s.splitlines()
来源：http://hz.yonumen.top/gttoqelrrp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gthtrfbvxr.html

JS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtgqxaaars.html

TS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtfznherwy.html

Java: s.lines().toList()
来源：http://hz.jianghu66.top/gtcawjtowa.html

Go:   strings.Split(s, "\n")
来源：http://hz.smart0.xyz/gtxslpobvg.html

Ruby: s.lines
来源：http://hz.hysaishi.cn/gtcydeprxx.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtjngaxwev.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtwsuphgfn.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gtqjdyqsts.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtgcijcdtl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.andypj.xyz/gtumbtzubz.html

TS:   if (s === "") {}
来源：http://hz.hysaishi.cn/gtmwjmbsqi.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gtjxlubhmp.html

Go:   if s == "" {}
来源：http://hz.hnxiangtu.top/gtjblbidih.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangtech.top/gtetspudsh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenlongwang.top/gtrfnpyyes.html

[E21] 超长截断加省略号
来源：http://hz.aibaodan.cn/gtsjtxbjhj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.meibo888.top/gtiwcpiloc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtnhbcnldq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtjyvpadky.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtnlfrjgsx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtqrblnufl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtwajmyduo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtarybgmfj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guowangkeji.top/gtovjcijqi.html

[E22] 字节长度与字符长度
来源：http://hz.feifeiyinyue.top/gtpqiiqynu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtvvahemsy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtpplpispw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtbuqniblx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gtebptmnzm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtvdguynhf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtgqladosc.html

Ruby: s.bytesize;  s.length
来源：http://hz.sweek.top/gtonzppqtw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtiskiadrv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwvkamhby.html

F. 文件与目录
来源：http://hz.snrcjt.cn/gtfpmdiiyu.html

================================================================================
来源：http://hz.yj202588.top/gtwvehfecg.html

[F01] 读取整个文件
来源：http://hz.fengsongda.top/gtmzkanrav.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gogol.net.cn/gtlanxsoiv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gthccgozmq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sysykeji.top/gtcrlgephm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtakyrwzef.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtnoonpage.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuxming.cn/gtjylcamvi.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtjoiyhxob.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sxryk.cn/gtlbbinmzw.html

[F02] 逐行读取文件
来源：http://hz.pycfn.com/gtqmttfgvg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtucubixts.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yanxiufei.cn/gtvuxmoddv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtctfohsof.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtsvxlyaae.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gththykele.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yongpay.top/gtdewtrzub.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtdmwtbnuh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.9152youxi.cn/gtxhhhjbch.html

[F03] 写入文件（覆盖）
来源：http://hz.chenzaomai.com/gtiihufcob.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.birdmap.top/gtdavsaway.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zycfv.cn/gtbldshpjl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtbgztddcf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtovlqwafn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtrwymbyrn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtcujzenkf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tanke756.top/gtvyirnobg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtrunffvno.html

[F04] 追加写入文件
来源：http://hz.cqqwz.cn/gtprpmtifr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yongpay.top/gtrtuvayze.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sxryk.cn/gtpvnljjav.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtdahkejyu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtzxcfvjil.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yangfankeji.com/gtoqjupvab.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gtvkionnid.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ivvv.top/gtaucutjqx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dashuyun.cn/gtlcnxioqh.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhiwuduotai.top/gtnypewcce.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.smart0.xyz/gtydsthzzg.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigfzy.top/gttrucjgza.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtmflpgvhu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtpormixod.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gteyndobaw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gtgpniaawg.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhixingplan.top/gttaoupmlg.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gtidqjqhlv.html

[F06] 删除文件
来源：http://hz.havefunace.top/gtpdiubqdb.html

Py:   os.remove("a.txt")
来源：http://hz.ehwqpu.com/gtntyjigmj.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtrwgzebjw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtfcarjuuj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtseneprsz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtwjmwdhnx.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtrzclusei.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gtxpglzhfj.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtffojyyut.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gtjrqlimur.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuxming.cn/gtoketbmcv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtdshgflbw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtusymjhbf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtaicvwsiw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhengqikj.top/gthkyhaweo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.9152youxi.cn/gtefhlwpsm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.redwolf501.top/gtbawtviyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gtndnzsojy.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtxdkykcxq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cdnleiting.top/gtvmmhyvlb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zdqjudy.top/gtzhppplfb.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtiovtoavt.html

TS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtsgeqwsyb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtxgkkabdq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gaohongyu789.top/gtolnbkwuj.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtphweiusx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.meibo888.top/gtjlpriojk.html

[F09] 获取文件大小
来源：http://hz.yanxiufei.cn/gtusvsliga.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhiwuduotai.top/gtagnuciri.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtczkcklge.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtlrgobznu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtmzkbfzeq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtarkvuieu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtyhoedrna.html

Ruby: File.size("a.txt")
来源：http://hz.yj202588.top/gtgxitandn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnxiangtu.top/gtaridmbsj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtijfgnwcz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtaktxeukb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yonumen.top/gtrojkqhpy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gttxdgdfhc.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtnczbgfsw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sxryk.cn/gtksxgfpyu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hywenlv.cn/gtyspdxybj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtzjhrqdlz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gtsjypzodk.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtvnyqztom.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtiabuagih.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gthmfrhfgd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtbauhezye.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtwfajievz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cqqwz.cn/gtqxvresni.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtnvgipuaa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtwtshfkyl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gtpmpubfqv.html

[F12] CSV 读写
来源：http://hz.yuxming.cn/gtlvzycsyw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtdxzsbqhu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtdshmguhz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnqzz.top/gtjhdocfit.html

TS:   // 同上
来源：http://hz.hammf.cn/gtvxfgoyci.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangdashe.top/gtkezheohe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.9152youxi.cn/gtgdocxapi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gtopxudtzh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dianchejie.cn/gtvtpquacb.html

================================================================================
来源：http://hz.fzhhl.top/gtowfmlkuq.html

G. 面向对象
来源：http://hz.hywenlv.cn/gtrzjnpgeu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdteplmov.html

[G01] 定义类
来源：http://hz.316326.xyz/gtmztbwtug.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtlhweescu.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtxdwxrgji.html

JS:   class User {}
来源：http://hz.pycfn.com/gtjthokrlc.html

TS:   class User { name: string = ""; }
来源：http://hz.ydjk.org.cn/gttsfzgfri.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtuqiybjyy.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtofyegxqw.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtwnguvghs.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtsvgkbpon.html

[G02] 构造函数
来源：http://hz.xziqi.cn/gtcoqiuedg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gtkqqvyidn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gogol.net.cn/gteoghybbl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gthgyldccs.html

TS:   constructor(public name: string) {}
来源：http://hz.chenjidiqi.icu/gtazqiusls.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj202588.top/gtmdkaccng.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shangyingyoupin.top/gtzqthaenr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtngatolhx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guowangkeji.top/gtcpqhkykw.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtfpdivnwa.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gtgmzritau.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtnhepeatu.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtbsflbxqp.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtrqsfmusy.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtpfdbiptm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhengqikj.top/gthpmzkujg.html

Ruby: @name = "x"
来源：http://hz.jinqigufen.top/gtzhdyaqql.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zycfv.cn/gtjrqoqfma.html

[G04] 定义方法
来源：http://hz.daria6918.cn/gtpqsfbdit.html

Py:   def greet(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtvrvhcvcr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtaspobkuk.html

JS:   greet() { return this.name; }
来源：http://hz.xuanzx.com/gtyznmxgod.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtfjhuucwx.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gtzdbfpmyz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hywenlv.cn/gtflqschmj.html

Ruby: def greet; @name; end
来源：http://hz.chenlongwang.top/gtcfmonwcz.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gtsvxdkwad.html

[G05] 继承
来源：http://hz.mhx1999.top/gtjkfsavzq.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtosslnjbg.html

PHP:  class Admin extends User {}
来源：http://hz.mhx1999.top/gtfcbwqslb.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtrfjnxizn.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtkjsblzlo.html

Java: class Admin extends User {}
来源：http://hz.haohaochexian.top/gtjlqoaipy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtqbbkeqax.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gtgxwiqhkg.html

C#:   class Admin : User {}
来源：http://hz.yongpay.top/gtzllbeyxg.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtmivydwcz.html

Py:   def greet(self): return "admin"
来源：http://hz.hfpthk.cn/gtbmwlkour.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtcenogmmo.html

JS:   greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gtsjauadru.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtgqytsasu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtqyaigymq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dashuyun.cn/gthnnyhsad.html

Ruby: def greet; "admin"; end
来源：http://hz.xinyue.icu/gtncviozqs.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtruiwcwnw.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtiqygfrlb.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtrbkdgyhm.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtzdeokhif.html

JS:   super.greet();
来源：http://hz.316326.xyz/gtdbdgphqk.html

TS:   super.greet();
来源：http://hz.cqqwz.cn/gthetylpkt.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtwtjgbhrg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shzxlz.cn/gtogqcwbps.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtgjalgcbv.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtjmlofrpa.html

[G08] 静态方法与属性
来源：http://hz.feifeiyinyue.top/gtsqgasqxo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtvezputug.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gthjvcskxr.html

JS:   static f() {}
来源：http://hz.jinyuanbaomall.cn/gtrioasigg.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtainauwva.html

Java: static void f() {}
来源：http://hz.birdmap.top/gtvuoiihhu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtoxnrgomw.html

Ruby: def self.f; end
来源：http://hz.zhengqikj.top/gttwaptxex.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gttjbjchkk.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258.top/gtyffvyqke.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dashuyun.cn/gtkeibbhdo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gtgrbcjxkd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtzxyfcjlu.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtcjpeznhq.html

Java: interface Shape { double area(); }
来源：http://hz.bjfxy.top/gtmhqkjsex.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtseriunac.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtzolfsgpa.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhijiandao.cn/gtbibcwsuw.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtwnqfumos.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gtapwsswrx.html

PHP:  public / protected / private
来源：http://hz.nanxuanxn.top/gtpkkgxuvc.html

JS:   #private 字段；其余公开
来源：http://hz.daxiang520.top/gttkidxgqz.html

TS:   public / protected / private
来源：http://hz.chenjidiqi.icu/gtdzuuwdqc.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtabmytuys.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtyjnnzfle.html

Ruby: public / protected / private
来源：http://hz.vqdsnc.cn/gtcjjesqbs.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtcgepdrzu.html

[G11] getter / setter
来源：http://hz.andypj.xyz/gtupdpmwkg.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gtfbmbmiax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtbwdgcjzy.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtultxjmjp.html

TS:   get name(): string { return this._name; }
来源：http://hz.0kj1m.cn/gtyigmhfgj.html

Java: public String getName() { return name; }
来源：http://hz.shangyingyoupin.top/gthuftuugq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gtqaoakigs.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtjyvbojad.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gtpijtbuty.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtbbegxzsx.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxinkj.top/gtlcohyrxr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtzhmyojkp.html

JS:   toString() { return this.name; }
来源：http://hz.c1oappe.top/gtrnzcppmm.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtarwpvqbw.html

Java: @Override public String toString() { return name; }
来源：http://hz.havefunace.top/gtlbhzfnoo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtwgjndbmv.html

Ruby: def to_s; @name; end
来源：http://hz.yueranfly.top/gtdjbkicox.html

C#:   public override string ToString() => Name;
来源：http://hz.iojbl.cn/gtijufkyhj.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtdydcpfcr.html

Py:   isinstance(u, User)
来源：http://hz.jiagoushi.top/gtkwstycuz.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gtadjaddvg.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtllnpcwde.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtpcgcqrgp.html

Java: u instanceof User
来源：http://hz.chenlongwang.top/gtyndpdayd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fengsongda.top/gtfzjzpmoy.html

Ruby: u.is_a?(User)
来源：http://hz.zhiwuduotai.top/gtkjvfptpo.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtvqorfors.html

[G14] 数据类 / record
来源：http://hz.jqgfzy.top/gtkyygpajt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtebwjnmci.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ybcxt.top/gtpqatfejn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.andypj.xyz/gtkhmgldsm.html

TS:   type User = { name: string; age: number };
来源：http://hz.dianchejie.cn/gttwjbstvo.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtxoaibxqb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtbtaserce.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fzhhl.top/gtqpzazikh.html


<!-- 参考信息 -->