代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtpyxrhhrz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtejyzmjms.html

C#:   1234567.ToString("N0")
来源：http://hz.smart0.xyz/gtaqwezodq.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtpnlzqpqn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gttclyhrck.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtavwukzkj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtkwkudqlv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtdnelhvdx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hywenlv.cn/gtuguasdks.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtjdmhivik.html

Ruby: s.capitalize
来源：http://hz.iojbl.cn/gtjfjyowxw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pycfn.com/gtqtitoxmj.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gtuycawxhh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gtzoyxahjg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenjidiqi.icu/gtjvwyehwh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtfekcmsnt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtkcfmkksy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tanke756.top/gtlecsevdn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dianchejie.cn/gtcqwnncdt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtvdmwnyzg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xylfe.cn/gtvlaewpso.html

[E19] 多行文本按行拆分
来源：http://hz.ydjk.org.cn/gtddzepell.html

Py:   s.splitlines()
来源：http://hz.hysaishi.cn/gtzdolppno.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ywan-chungtsiang.top/gtqnohtlpi.html

JS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtdzofhzgb.html

TS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtrewokqch.html

Java: s.lines().toList()
来源：http://hz.feifeiyinyue.top/gthojzpaun.html

Go:   strings.Split(s, "\n")
来源：http://hz.9152youxi.cn/gtwrsaafle.html

Ruby: s.lines
来源：http://hz.9152youxi.cn/gtmwkgsaoc.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtlqnpoebn.html

[E20] 判断字符串是否为空
来源：http://hz.shangyingyoupin.top/gtlgtvqcjq.html

Py:   if not s:
来源：http://hz.jinqigfzy.top/gtkqvyjilv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.havefunace.top/gtdgaylhlq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtgotloczr.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtxplunhyf.html

Java: if (s.isEmpty()) {}
来源：http://hz.pycfn.com/gtsumrykaq.html

Go:   if s == "" {}
来源：http://hz.zhoulong.xyz/gtfoybunst.html

Ruby: if s.empty?
来源：http://hz.yangfankeji.com/gtsfuzegrd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.svipenyu.cn/gtrjhwhfna.html

[E21] 超长截断加省略号
来源：http://hz.jqgufenzy.top/gthpxdqhqq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtvhlucywj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gtqbvfyiaw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtxcrdfaxl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtrekderun.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtrhurevyi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gttyuxtgzq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aizwys.cn/gtkbiwukcp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtemnvpfeg.html

[E22] 字节长度与字符长度
来源：http://hz.ehwqpu.com/gtbhsfwwjc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ywan-chungtsiang.top/gtlyrvqgnh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtoadnyydb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gttgtazrfo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtkdnxwtfi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtadebvjfu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yongpay.top/gtfrvhnyzg.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gtiswtssmt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gotoacloud.top/gtipwwwtjq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtyaqmmlwz.html

F. 文件与目录
来源：http://hz.yanxiufei.cn/gtfspnjwek.html

================================================================================
来源：http://hz.snrcjt.cn/gtorotwquw.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtehzgtdpr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtqcfobxac.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtdkuysgvu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daria6918.cn/gtkkxfjzpk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.vqdsnc.cn/gtrmztidkr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtxobpfwjw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhixingplan.top/gtqethzsfk.html

Ruby: File.read("a.txt")
来源：http://hz.aibaodan.cn/gtkvugyfxv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xylfe.cn/gtzjtgacgd.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtaijxvjgq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtaubgvkan.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtbafwbgwp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gtkhyffkwm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gtapmtndcq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtscmqzcag.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sweek.top/gtmbhslczn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtdzektwib.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhongyouzk.top/gtcyqnpask.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtzeiuuejg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtsrqzbyhm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtmimixarq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gttjtgordu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtdvqgqxnt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtmgobdmtc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxinkj.top/gthioczseq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtaktgzgqg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtmgjsyfve.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtjlziguzw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pengpengdd.cyou/gthqibases.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtkaydwyla.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtorxdigko.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtgccafjpt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xinyue.icu/gtztkfxaai.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gttsocqoev.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhixingplan.top/gtaitflula.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gtrfcapoxx.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gtzbictreq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ppjwa.cn/gtpbqhaacv.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtwsnksuha.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtmrjvyfqr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtegrlkreu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtxeesksic.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigufen.top/gtedurvvjz.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtfnbpmzrj.html

C#:   File.Exists("a.txt")
来源：http://hz.cdnleiting.top/gtrmvhaxrf.html

[F06] 删除文件
来源：http://hz.svipenyu.cn/gtsozsbwaf.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gttgrxvtfy.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtmgkncvex.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtuuigujyy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sysykeji.top/gtifjhhttd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtkpwvsbux.html

Go:   os.Remove("a.txt")
来源：http://hz.tian-w.cn/gthdjvbqrk.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtiyaulcwf.html

C#:   File.Delete("a.txt");
来源：http://hz.cashguo.top/gtipcuehzg.html

[F07] 创建目录（含多级）
来源：http://hz.ivvv.top/gtpcgkdumn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtdvsomysx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cdnleiting.top/gtmoayrwkn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtkeruchre.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtavrxuwte.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtgqjnpijy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtxkjxsmmz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gteiwlppmc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sysykeji.top/gtgrirzbst.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gtfxhdgtwj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtuxlluubx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hammf.cn/gtoskizbtg.html

JS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtyeobymsg.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtyfwvtnzw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtnljckflz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtdoxtcusr.html

Ruby: Dir.children("dir")
来源：http://hz.shuidangran.top/gtszonlzfo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dianchejie.cn/gtvhwrmnwd.html

[F09] 获取文件大小
来源：http://hz.chenjidiqi.icu/gtorxfldzc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gtdbpjuxvf.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtyxlywtnm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtisbzjtub.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtpmedezrp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtuecusebl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtttbmrxvl.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtgmgiczud.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtpadwijvj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xziqi.cn/gtgnhtmdaw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtjvlbtitf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xziqi.cn/gtntkbqsmw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtbeqywehj.html

TS:   path.extname("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqnmeaxdu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtrljfnmtx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sweek.top/gtpwacuklx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gttglpiwrw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtmylntgjk.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtllkutori.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtnjdrkjnh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sxryk.cn/gtdszafyzo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtnqmycmga.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gttwhadrkx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtkumrotye.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gttdlzbfzy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtpvvtahrg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.52xcode.cn/gtgkparwci.html

[F12] CSV 读写
来源：http://hz.havefunace.top/gtlgswozrf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cucudq.cn/gtepwdksvx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtumoqsbhh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangdashe.top/gtxdbdmoqr.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gthtylzkcc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.52xcode.cn/gtaqvywbbi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtmwoycikj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zycfv.cn/gttaeapoyz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cheryme.top/gtrdxijcna.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtggjhhezt.html

G. 面向对象
来源：http://hz.jinghuilouyu.cn/gtcvoqtwjg.html

================================================================================
来源：http://hz.meibo888.top/gtgupyyloa.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtvstmxole.html

Py:   class User: pass
来源：http://hz.ybcxt.top/gtjbnxukti.html

PHP:  class User {}
来源：http://hz.gaohongyu789.top/gtrehqqjth.html

JS:   class User {}
来源：http://hz.cucudq.cn/gtwvritsoi.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtjzpwkrek.html

Java: class User {}
来源：http://hz.sysykeji.top/gtequrauja.html

Go:   type User struct { Name string }
来源：http://hz.gzhubu.top/gtcaqyacoy.html

Ruby: class User; end
来源：http://hz.yuxming.cn/gtjllrnzva.html

C#:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtadmmfnyf.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gthprfnabs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtflomizqd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.quarkkingdee.top/gtjazfqpwl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtqfcyczew.html

TS:   constructor(public name: string) {}
来源：http://hz.0kj1m.cn/gtupzojhju.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gtaksdoijl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.redwolf501.top/gttvmcvsun.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangshuangyany.cn/gtabqfubwf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xziqi.cn/gtihhtoroe.html

[G03] 实例属性
来源：http://hz.nanxinkj.top/gtdmsptkub.html

Py:   self.name = "x"
来源：http://hz.yangfankeji.com/gtxjqrmise.html

PHP:  public string $name = "x";
来源：http://hz.dianchejie.cn/gthdiczesz.html

JS:   this.name = "x";
来源：http://hz.gaohongyu789.top/gtfekvvump.html

TS:   name: string = "x";
来源：http://hz.cqqwz.cn/gtblqphlrc.html

Java: private String name;
来源：http://hz.quarkkingdee.top/gtizsswsln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yvedp.cn/gtqqqnasph.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtknfemfse.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtsmxgevpa.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gtlisbdodo.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtmvmoarwv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtssgahwpo.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gthptipnsx.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuxming.cn/gtxynkegnr.html

Java: String greet() { return name; }
来源：http://hz.zhoulong.xyz/gtttgqlrab.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtjseigzkl.html

Ruby: def greet; @name; end
来源：http://hz.zhixingplan.top/gtrbcgdfnt.html

C#:   public string Greet() => Name;
来源：http://hz.hfpthk.cn/gtwmitmcqg.html

[G05] 继承
来源：http://hz.hfpthk.cn/gtsnyumkxr.html

Py:   class Admin(User): pass
来源：http://hz.haohaochexian.top/gtjmyyeqgk.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtfqpwmspb.html

JS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtxiyxmkql.html

TS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtzfnayiwi.html

Java: class Admin extends User {}
来源：http://hz.andypj.xyz/gtatppihwf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtvxnzdyrf.html

Ruby: class Admin < User; end
来源：http://hz.mhx1999.top/gtgohtmfpa.html

C#:   class Admin : User {}
来源：http://hz.birdmap.top/gtzlctimqw.html

[G06] 重写方法
来源：http://hz.yuanzhike.top/gtqmsxeyra.html

Py:   def greet(self): return "admin"
来源：http://hz.chenlongwang.top/gtjikcnuui.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtqbehrtvp.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtyfsatgyh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtitefzgyx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtgnffzvpi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenzaomai.com/gttdvqpsfr.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtlxekbzid.html

C#:   public override string Greet() => "admin";
来源：http://hz.kuanghao11.cn/gtbabxxjkg.html

[G07] 调用父类方法
来源：http://hz.yuxming.cn/gtlrtqqqau.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtcjtzynue.html

PHP:  parent::greet();
来源：http://hz.hnxiangtu.top/gtkztdjhlm.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtntjohqdd.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtworapxsv.html

Java: super.greet();
来源：http://hz.ywan-chungtsiang.top/gtguoofkku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuxming.cn/gtanstxcdv.html

Ruby: super
来源：http://hz.chenzaomai.com/gtuzpjnzbw.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtsuyxpwaw.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gttpwsyxwt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yvedp.cn/gtirbwapnt.html

PHP:  public static function f() {}
来源：http://hz.yonumen.top/gtudvixmlc.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtlenfcsau.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtmelojhin.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtgwzwzfon.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.birdmap.top/gtmbgzkuvi.html

Ruby: def self.f; end
来源：http://hz.ydzc1.top/gthoxkuoxz.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtnspcjuvd.html

[G09] 接口 / 抽象类
来源：http://hz.snrcjt.cn/gtexhavgle.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtotnjquqi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhoulong.xyz/gtqryavotr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gtqxbqzgon.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtvfnzymer.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtmfmmksje.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenjidiqi.icu/gttqoyiawj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtaadzvlnz.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinyuanbaomall.cn/gtpilopgie.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtncenxipr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtmbbbpgdy.html

PHP:  public / protected / private
来源：http://hz.sweek.top/gtzldpasip.html

JS:   #private 字段；其余公开
来源：http://hz.smart0.xyz/gtdsgxwvcy.html

TS:   public / protected / private
来源：http://hz.tian-w.cn/gthxtdwnnp.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtlibdunpj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtqucbigcv.html

Ruby: public / protected / private
来源：http://hz.jinghuilouyu.cn/gtpidhpzau.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtzongahvh.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gtrklisrvd.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gthvjyskkc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtmeqllsbv.html

JS:   get name() { return this._name; }
来源：http://hz.shangyingyoupin.top/gtmzodvivr.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtmpjdkehe.html

Java: public String getName() { return name; }
来源：http://hz.daria6918.cn/gtjwfvkbgf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jianghu66.top/gtsuczmghc.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtxxqhlznv.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtndkakycy.html

[G12] 对象转字符串
来源：http://hz.chenlongwang.top/gtrswmsfst.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtwpqpdbmi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtnvpfvkiw.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gtjosxmnqa.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtlsnssqrw.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhoulong.xyz/gttqovtaso.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtfnwckddp.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gttkxpbtks.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtelkoxgoi.html

[G13] 判断对象类型
来源：http://hz.zhengqikj.top/gtqvuzkoor.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtvhbjthdp.html

PHP:  $u instanceof User
来源：http://hz.jinqigfzy.top/gtkamynmad.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtpfhusaed.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtktcsqeiv.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtkyctutgh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtrqbzenzo.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigfzy.top/gtlnjdflhr.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtwicabxxd.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtpaofmnlr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtepvhkjam.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jiagoushi.top/gtjgczgrkr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gtwisqxqqr.html

TS:   type User = { name: string; age: number };
来源：http://hz.havefunace.top/gtpifgypin.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtzsnjfszc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gthzaoumgv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hysaishi.cn/gtgtmvgoul.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gtygjwtrqy.html

[G15] 枚举
来源：http://hz.0kj1m.cn/gtalrdeovb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yanxiufei.cn/gtwmgqkgxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtahgdotkn.html


<!-- 参考信息 -->