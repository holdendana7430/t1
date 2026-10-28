代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guowangkeji.top/gtwyldooxb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.snrcjt.cn/gtkgfqtmys.html

C#:   1234567.ToString("N0")
来源：http://hz.pycfn.com/gtulrghcqb.html

[E17] 首字母大写
来源：http://hz.sysykeji.top/gtymhddidl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtgfbbleng.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtnmjnqqzz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtnkiigjdu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtjsteoljd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtiwdypvpu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtishpqxja.html

Ruby: s.capitalize
来源：http://hz.svipenyu.cn/gtatkbkmnb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.guowangkeji.top/gtqdupepoh.html

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gtahrkfruv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangdashe.top/gtygseikpl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.52xcode.cn/gtwjefqkwz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtcdmzcqsw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gthmivrhms.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtdbjbfujf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.bjfxy.top/gtdopqhtkr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtohkxhhdz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cashguo.top/gtgeeikavy.html

[E19] 多行文本按行拆分
来源：http://hz.xuanzx.com/gtxsbcdega.html

Py:   s.splitlines()
来源：http://hz.hfpthk.cn/gtlnlemono.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tian-w.cn/gtphgvqylz.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtpvrsfykk.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtzvhqwuaj.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gthihttaey.html

Go:   strings.Split(s, "\n")
来源：http://hz.guowangkeji.top/gtmjneoutt.html

Ruby: s.lines
来源：http://hz.zycfv.cn/gtmcaasyoy.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtyvaxtwxv.html

[E20] 判断字符串是否为空
来源：http://hz.hammf.cn/gtjxyofcsr.html

Py:   if not s:
来源：http://hz.ivvv.top/gtpdibusej.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtjtewspwf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.bjfxy.top/gtagqdwyqb.html

TS:   if (s === "") {}
来源：http://hz.tanke756.top/gtkqzgrflc.html

Java: if (s.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtyrsfnvku.html

Go:   if s == "" {}
来源：http://hz.316326.xyz/gtxxowrnmy.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtctlqnlpe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gttqdlbsmm.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtdlrxdlte.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gtxsjlimsq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shzxlz.cn/gtddxddipv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtoezguqjd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtyfdlsiqs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtjmgknakq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sysykeji.top/gtbtzclajc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gtkysquqkr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgufenzy.top/gtahfprsmz.html

[E22] 字节长度与字符长度
来源：http://hz.snrcjt.cn/gtersjdhnt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinyuanbaomall.cn/gtcfluksud.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtspgozweg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gthmbqnekh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gthugyhing.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guowangkeji.top/gtacqswwov.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cqqwz.cn/gtkqryeknq.html

Ruby: s.bytesize;  s.length
来源：http://hz.havefunace.top/gteywxrlip.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hnqzz.top/gtpcehtfvo.html

================================================================================
来源：http://hz.zhoulong.xyz/gtaubbvgyr.html

F. 文件与目录
来源：http://hz.c1oappe.top/gtqlkmekbi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtqckzfejb.html

[F01] 读取整个文件
来源：http://hz.ywan-chungtsiang.top/gtlevthgeh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jyoumei.cn/gtwdbqwflq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yanxiufei.cn/gtkchrxyrc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtlramhptz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigufen.top/gtqvkzzata.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtmokkyunn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cqqwz.cn/gtlhwpdbgt.html

Ruby: File.read("a.txt")
来源：http://hz.ivvv.top/gtrfzobuak.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gthewchxnh.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtskjbmkqv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gttayamqwr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gtmsnowsgp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtxkuhubqt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtzoxaghbf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtlatzfcbb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gthuucjtdl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtblmtdeuk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cqqwz.cn/gtdnhmccvd.html

[F03] 写入文件（覆盖）
来源：http://hz.hammf.cn/gtizrosegu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhixingplan.top/gthlsrgpwh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtvmhdjdks.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtgnsoiazg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtgjxaeuvc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtlhtfmcqj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtrzsujcfl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtkahhyeur.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj202588.top/gtdjwnfuax.html

[F04] 追加写入文件
来源：http://hz.chenjidiqi.icu/gtsiphzyhc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sxryk.cn/gtvhlqplel.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhiwuduotai.top/gtdbvvbhjk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtpxgypalf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dianchejie.cn/gtivfqjsqn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtjamhodkq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtikjymdzb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtjenkcmgu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.birdmap.top/gtrcxvowyp.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnxiangtu.top/gtjxtyoqwp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydjk.org.cn/gtuvrtcqye.html

PHP:  file_exists("a.txt");
来源：http://hz.ppjwa.cn/gtsgsfrueq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtsecrkzvn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtxfuvrkhb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gterrbbtuf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangshuangyany.cn/gtztyxzinw.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdyqjqkru.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtammzrmbh.html

[F06] 删除文件
来源：http://hz.hongshengwenyu.top/gtwionlmkp.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtmywcfdns.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtwqfodcsb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sysykeji.top/gtiigjjcrn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtktelgciz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtblkeuatx.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgufenzy.top/gtheqbarnl.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtvxodsmma.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gtrbbakcne.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtlzjibfnn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gogol.net.cn/gtzmmdndio.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yvedp.cn/gtrdhqqjne.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtatuqofbs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtpdwwplfn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sysykeji.top/gtxmxubshg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.haohaochexian.top/gtgbdzkcgi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yonumen.top/gtrnmujath.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtlughzwds.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gttprjpkwv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhoulong.xyz/gtyllyjwaa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gtaprlgpqb.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtnltnzmpk.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhongyouzk.top/gtvdghcfzp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtlrjtxpby.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxuanxn.top/gtmwdyscws.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtfyturpbb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtrvywsahw.html

[F09] 获取文件大小
来源：http://hz.nwbrower.top/gtdoykhskz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gttmgfqdhm.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtzvozlwzs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gtalfwqmsn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtwavwwztn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtqwrotoau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gtulzmneiy.html

Ruby: File.size("a.txt")
来源：http://hz.52xcode.cn/gtuoncozpt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtwvmjunom.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gtsurpbdvk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtogmwycam.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtpeolggug.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtcxlzrusx.html

TS:   path.extname("a.txt")
来源：http://hz.pengpengdd.cyou/gtwfcpqdlv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtbuxwwkfh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtenkmpgkf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtdurhsoec.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtnwhdzidf.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtjhyxxfgw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtivoelhtq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xingfuxueyuan.xyz/gtrtdajraw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtgzvwltgd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtiidempht.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gzhubu.top/gtlyyynuxp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtrveoougu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtiwueabyb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtfpcbladm.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gtfwhvpbvm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gttbqcnziw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gttbwbwgre.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtzfamapko.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtcvpchaeh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gaohongyu789.top/gtfnpoauou.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.birdmap.top/gtihflcxtv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gtbrqwpalo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jlsjyb.cn/gtsgqtrlth.html

================================================================================
来源：http://hz.iojbl.cn/gtbnfinjrj.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtiuvocjur.html

================================================================================
来源：http://hz.zhongyouzk.top/gtylfghmvn.html

[G01] 定义类
来源：http://hz.tanke756.top/gtqmcmgcwa.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtvjkfgcjg.html

PHP:  class User {}
来源：http://hz.svipenyu.cn/gtszmbtguv.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtohdzsxnc.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtnkcpbvma.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtfhwkhdoh.html

Go:   type User struct { Name string }
来源：http://hz.yj20258.top/gtezluccjy.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gtrqeyfszv.html

C#:   class User {}
来源：http://hz.chenzaomai.com/gtiicqnifp.html

[G02] 构造函数
来源：http://hz.yuxming.cn/gtwyotihku.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aizwys.cn/gtyusorima.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtcrkhwtxy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtneuyokto.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gtmiselypz.html

Java: User(String name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtwkhqtxtt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtqltibquh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtmjmbsjgq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuetiantiany.cn/gtefiunvuk.html

[G03] 实例属性
来源：http://hz.jinqigufen.top/gtsizxgtjz.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtfwroxapy.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gtuvhntngg.html

JS:   this.name = "x";
来源：http://hz.jianghu66.top/gtwphbufjb.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtbsosxzvv.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtvoybpdim.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhoulong.xyz/gthmjlowiy.html

Ruby: @name = "x"
来源：http://hz.nwbrower.top/gtfkfroyrc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtpyvaxuas.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gtzxnutcfq.html

Py:   def greet(self): return self.name
来源：http://hz.pycfn.com/gtnftobjov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtgwfmomrg.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtvrrqxryi.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtyzllmbvi.html

Java: String greet() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtcdiuigmt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtlnlrxlpj.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gtuujlgepn.html

C#:   public string Greet() => Name;
来源：http://hz.xuanzx.com/gtwlhficak.html

[G05] 继承
来源：http://hz.daxiang520.top/gtwmiiqpmb.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtuixnoeis.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gtshqgxdzt.html

JS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtqgbvnopq.html

TS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtovukmquh.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtezzgcyrz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtbinryioj.html

Ruby: class Admin < User; end
来源：http://hz.ydzc1.top/gtaxyovuij.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtwkluytra.html

[G06] 重写方法
来源：http://hz.xuanzx.com/gtixnokwoo.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtyviayreb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtafvgloqz.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtmkzhrypi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtujpfpaso.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtkuylaffd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daxiang520.top/gtufaeppcl.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtkwuljbqf.html

C#:   public override string Greet() => "admin";
来源：http://hz.gotoacloud.top/gtbxtsufen.html

[G07] 调用父类方法
来源：http://hz.andypj.xyz/gtvcwviwjl.html

Py:   super().greet()
来源：http://hz.yonumen.top/gttmisaqqm.html

PHP:  parent::greet();
来源：http://hz.chenjidiqi.icu/gtcwqrdxys.html

JS:   super.greet();
来源：http://hz.sysykeji.top/gtezqtfybm.html

TS:   super.greet();
来源：http://hz.yuxming.cn/gtwnswrypk.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtvlfdjvoo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gtpubiwccd.html

Ruby: super
来源：http://hz.shzxlz.cn/gtftnxabgp.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtfdfklttm.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtnvbkkrbb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.bjfxy.top/gtkbaulttg.html

PHP:  public static function f() {}
来源：http://hz.0kj1m.cn/gtosflzjyd.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gttrgadlex.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtirfzqzyh.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtcdqsyntr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtpvuhrcar.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gtphmgdsej.html

C#:   public static void F() {}
来源：http://hz.gaohongyu789.top/gtzvayyihb.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtpbeetayc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtqjdwxpea.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtzrtzfewd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jyoumei.cn/gtzrekobep.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtcexuxvim.html

Java: interface Shape { double area(); }
来源：http://hz.ydzc1.top/gtfkjdvnuh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xziqi.cn/gtxdynbfeg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtvnfdvqbj.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtuukfrrwq.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtxwhujfaf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtyzdlegyh.html

PHP:  public / protected / private
来源：http://hz.yuanzhike.top/gtbkdwrhxk.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtkxglhmbw.html

TS:   public / protected / private
来源：http://hz.sxryk.cn/gtgwgojppd.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtkfhyriyw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtihpupgwi.html

Ruby: public / protected / private
来源：http://hz.zhoulong.xyz/gtglvzwtwy.html

C#:   public / protected / private / internal
来源：http://hz.aizwys.cn/gtmynxyapr.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtthmtzdsa.html

Py:   @property 与 @x.setter
来源：http://hz.xingfuxueyuan.xyz/gtiupaende.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtlpedohhc.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtyvbrmbdn.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtavefnuaa.html

Java: public String getName() { return name; }
来源：http://hz.316326.xyz/gtbqdelzok.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtdnyvzwau.html

Ruby: attr_accessor :name
来源：http://hz.hnqzz.top/gtyxyrggbz.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtuogqlygt.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gtgotxveqg.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gtkbojrlaw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gttfbndkmz.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtuevzlzsd.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtlihcowcf.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtsuqlzqvo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gtqpurjmfb.html

Ruby: def to_s; @name; end
来源：http://hz.jiagoushi.top/gtfsvrlulc.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gtbyzbqymo.html

[G13] 判断对象类型
来源：http://hz.birdmap.top/gtfwjbmgba.html

Py:   isinstance(u, User)
来源：http://hz.quarkkingdee.top/gtcjkkpbao.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gttdpsrins.html

JS:   u instanceof User
来源：http://hz.ydzc1.top/gtyzaohcjm.html

TS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtsnrcfrtu.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gttsowxwtq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtqrfqaobh.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtvtqnsgia.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtvablsrhg.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtiouvptzu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gzhubu.top/gtwhyalhaa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ppjwa.cn/gttlwwedxl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtlyhrrgrv.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtluibihun.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtiualljbh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hongshengwenyu.top/gtevmugtjk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yvedp.cn/gtnipvohfq.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtyhunrhjn.html

[G15] 枚举
来源：http://hz.tanke756.top/gtqnunrorn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtabxffhwl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cheryme.top/gtiyvzrgro.html


<!-- 参考信息 -->