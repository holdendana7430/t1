代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zycfv.cn/gtnjwxqmnq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gtsgnhewhb.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gtxcdikblq.html

[E17] 首字母大写
来源：http://hz.chenjidiqi.icu/gtuujltbdz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtfjbumbhn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhoulong.xyz/gthavbrqvc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtarjeeakj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtrebjopix.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydzc1.top/gtecfrhqjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.c1oappe.top/gtgsremowm.html

Ruby: s.capitalize
来源：http://hz.gogol.net.cn/gtbgoerdzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hysaishi.cn/gtyyovjkjm.html

[E18] 模板占位符替换
来源：http://hz.havefunace.top/gtklyiifpn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gttyywnmkb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuxming.cn/gtiyaxddxj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtfmpgbvtt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtlnbtfhje.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtzskwmvqv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtkvlujjhp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenzaomai.com/gtqekvvktd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtvqegbpcm.html

[E19] 多行文本按行拆分
来源：http://hz.jinghuilouyu.cn/gtqvvgoguv.html

Py:   s.splitlines()
来源：http://hz.jyoumei.cn/gthugrumma.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tanke756.top/gtadtmxzrh.html

JS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtfygjghyp.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtgrkbrrpx.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gtcdrzatbi.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtviyiuaai.html

Ruby: s.lines
来源：http://hz.9152youxi.cn/gtykpwzftj.html

C#:   s.Split('\n')
来源：http://hz.zhengqikj.top/gtkzmmjwyb.html

[E20] 判断字符串是否为空
来源：http://hz.jyoumei.cn/gtcucqfeuz.html

Py:   if not s:
来源：http://hz.mhx1999.top/gtbuoacgbt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinyuanbaomall.cn/gtnjbcmwil.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhijiandao.cn/gtpbagnapn.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gthtjcznnn.html

Java: if (s.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtyhyxskxb.html

Go:   if s == "" {}
来源：http://hz.gzhubu.top/gtbexoqipt.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gtzwzmgway.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtscryoedt.html

[E21] 超长截断加省略号
来源：http://hz.jinyuanbaomall.cn/gtmboigrkw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuetiantiany.cn/gtevuzlcyj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtmmgassie.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtuozaosck.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtopfiqhvl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtzytkxerr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtavwncdfw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pycfn.com/gtqfewgpoc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zdqjudy.top/gtclqqcdqj.html

[E22] 字节长度与字符长度
来源：http://hz.zycfv.cn/gtgppvuuly.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gtmjacyrqu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtlhgfhhss.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtdebvhsug.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtoyqyekbc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuetiantiany.cn/gtetmmiimu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hysaishi.cn/gttaverlxq.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtzenotzme.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhiwuduotai.top/gtzhbfsdcc.html

================================================================================
来源：http://hz.aibaodan.cn/gtynukelto.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gtbtrzvgzu.html

================================================================================
来源：http://hz.cucudq.cn/gtottwygpr.html

[F01] 读取整个文件
来源：http://hz.pengpengdd.cyou/gtshseqyfz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhiwuduotai.top/gtsidviodx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj202588.top/gtdmpimkqq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtkzosnoxk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtvycnuuuh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtwffrvtfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guowangkeji.top/gtxflbcmqy.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtoydggqld.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.smart0.xyz/gtidptdyld.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtjlhbphuu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gtphnwnjyh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydjk.org.cn/gtlyizannm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtcjhhebss.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtlmgxvfki.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtkxrpwson.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtjrbpnony.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtpmouwdvb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.havefunace.top/gtkpbwvshq.html

[F03] 写入文件（覆盖）
来源：http://hz.ywan-chungtsiang.top/gtvlvzfrqd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtwliziabs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.c1oappe.top/gtpczrleyz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gtmuknnyib.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtmauhrlul.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gtoovtmlop.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xinyue.icu/gtihdbqrpz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtqmymodbd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cucudq.cn/gtjggffmys.html

[F04] 追加写入文件
来源：http://hz.jinyuanbaomall.cn/gtciuizqvl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cdnleiting.top/gtlfdlkgig.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ehwqpu.com/gtcmgglqok.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtvbpjocqg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtailoojxe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtfufvjadx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gotoacloud.top/gttpulsyer.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.smart0.xyz/gtwvzwaknd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gtwboehdvg.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtcmhimlff.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtpulmpspb.html

PHP:  file_exists("a.txt");
来源：http://hz.ppjwa.cn/gtkmmvueer.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtwzsygknq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtmrsbwafs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtduubnsmp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gthoidvvqi.html

Ruby: File.exist?("a.txt")
来源：http://hz.pengpengdd.cyou/gtgsgmriez.html

C#:   File.Exists("a.txt")
来源：http://hz.cdnleiting.top/gtipffibnf.html

[F06] 删除文件
来源：http://hz.jianghu66.top/gtvdhobxus.html

Py:   os.remove("a.txt")
来源：http://hz.ydjk.org.cn/gttbcsqqxe.html

PHP:  unlink("a.txt");
来源：http://hz.fengsongda.top/gtdtofrviw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtudqieigm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtcclwpuqm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtrsvggzkq.html

Go:   os.Remove("a.txt")
来源：http://hz.smart0.xyz/gtrdrpyfpe.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxuanxn.top/gtdjrukhtl.html

C#:   File.Delete("a.txt");
来源：http://hz.xziqi.cn/gteabhwpcj.html

[F07] 创建目录（含多级）
来源：http://hz.shuidangran.top/gtsiqochsw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gturpkkwce.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtpjljaeci.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtvrhvvyly.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtxjpaqhmf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtlfdcakcs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daxiang520.top/gtjginmgrm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pengpengdd.cyou/gtaqfhujya.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtfmrcjdhi.html

[F08] 遍历目录
来源：http://hz.pengpengdd.cyou/gtlfinjxyl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gtfxhsdrkt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cashguo.top/gtesekddey.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtvghhfyoj.html

TS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtmnqrbhku.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtjzeokqqt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.vqdsnc.cn/gtiizdznqu.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtwfeovffg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.kuanghao11.cn/gtphohdnua.html

[F09] 获取文件大小
来源：http://hz.ydjk.org.cn/gtxyxnjuhp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtribrrhwq.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gtkybracet.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dianchejie.cn/gtoerbocny.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtajabfpcz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtnpbecqym.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yanxiufei.cn/gtbpzvsoqu.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gtmirnfscb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hysaishi.cn/gtzdhwpjqv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtprebwclv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtmbxwscio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtdxmmefni.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtdebhexnr.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258888.top/gtvajpnsjk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtrpkkxsju.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtldwcftsr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtlvjbjkbf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guowangkeji.top/gtqysrtfcg.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gtsocxnqib.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtxshpokwl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtcoifhtoh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtixekqzkr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtnbgvlmfv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtpvfvyiak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigufen.top/gtyxwjlfgy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtabmhxsmv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gttpeqresw.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gtlaerulrj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xylfe.cn/gtkbzxyvom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sxryk.cn/gtzrawftxg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gttpoarkdo.html

TS:   // 同上
来源：http://hz.guowangkeji.top/gtdjhwtssa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258888.top/gtznwmxrua.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jianghu66.top/gthgmcmbpf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daxiang520.top/gtnothsmmw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtqxnpqcwa.html

================================================================================
来源：http://hz.cdnleiting.top/gttksqraju.html

G. 面向对象
来源：http://hz.yuxming.cn/gtkonxfulh.html

================================================================================
来源：http://hz.wangdashe.top/gtucdmlxyg.html

[G01] 定义类
来源：http://hz.xuanzx.com/gtftayzfew.html

Py:   class User: pass
来源：http://hz.svipenyu.cn/gtbwhsaotd.html

PHP:  class User {}
来源：http://hz.sweek.top/gtmyianboo.html

JS:   class User {}
来源：http://hz.c1oappe.top/gtmkennjtj.html

TS:   class User { name: string = ""; }
来源：http://hz.zycfv.cn/gtwohobtlr.html

Java: class User {}
来源：http://hz.fengsongda.top/gtgcrltzit.html

Go:   type User struct { Name string }
来源：http://hz.yuxming.cn/gtqvbumdiz.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtahkyvocu.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gthrhfswgt.html

[G02] 构造函数
来源：http://hz.jiagoushi.top/gttnmzenyn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtwacorboh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tanke756.top/gtlaeipniy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtplsieljg.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtisawcaic.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnqzz.top/gthghhbxtj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtqvyzugqq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yueranfly.top/gtopoeqdrz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnxiangtu.top/gtvxyugafb.html

[G03] 实例属性
来源：http://hz.yonumen.top/gtaonourmq.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtaesnyeas.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gtkkgeemod.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtgvcffrrh.html

TS:   name: string = "x";
来源：http://hz.316326.xyz/gtqmkrpzec.html

Java: private String name;
来源：http://hz.xinyue.icu/gtqzmbwums.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.52xcode.cn/gtxjedpdic.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtqvzeqsgj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hfpthk.cn/gtmsayhvar.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtvidthsxn.html

Py:   def greet(self): return self.name
来源：http://hz.wangshuangyany.cn/gtieauxnfz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtgvjotudg.html

JS:   greet() { return this.name; }
来源：http://hz.havefunace.top/gtelgplmbn.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtrkuxchdq.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtvkvphbrn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtweylahgn.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtezlystpp.html

C#:   public string Greet() => Name;
来源：http://hz.cdnleiting.top/gtmarrcjre.html

[G05] 继承
来源：http://hz.nwbrower.top/gtjajecugr.html

Py:   class Admin(User): pass
来源：http://hz.yj20258888.top/gtzbeopxkt.html

PHP:  class Admin extends User {}
来源：http://hz.chenlongwang.top/gtvjkbizkq.html

JS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtbufajfej.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtfrlffoif.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtpyyavgao.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258888.top/gthljusmke.html

Ruby: class Admin < User; end
来源：http://hz.fzhhl.top/gtbawbbwto.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gtadoxvmip.html

[G06] 重写方法
来源：http://hz.9152youxi.cn/gtejrguajz.html

Py:   def greet(self): return "admin"
来源：http://hz.chenlongwang.top/gtccnulzdw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtgidiyppf.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtzbvxgoay.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtknfwxluh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtmxxzdfko.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtfuuanach.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtkyyeqyul.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtbyebdtlu.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtmafnqeft.html

Py:   super().greet()
来源：http://hz.ppjwa.cn/gtpthvbgsl.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtdzsrvwbv.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtwduqrgcv.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtuybiqogo.html

Java: super.greet();
来源：http://hz.zhiwuduotai.top/gtxjdoeaab.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cheryme.top/gtyttncbpq.html

Ruby: super
来源：http://hz.xylfe.cn/gtjazuinmy.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtnmutenre.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtcyurutqa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtntuxaarf.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gtbfigenue.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gtcoaviueu.html

TS:   static f(): void {}
来源：http://hz.9152youxi.cn/gtigxgxfzk.html

Java: static void f() {}
来源：http://hz.c1oappe.top/gtetgbrjmf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sysykeji.top/gtotrreohk.html

Ruby: def self.f; end
来源：http://hz.jinghuilouyu.cn/gtuvkgusgl.html

C#:   public static void F() {}
来源：http://hz.iojbl.cn/gtlvonxgtf.html

[G09] 接口 / 抽象类
来源：http://hz.shuidangran.top/gttflnjzfh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtsgyytzev.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtycxoofqd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cashguo.top/gtlckldtdz.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtwzmrouts.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gtpbjndypn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zdqjudy.top/gtzxwuxeyp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtgarlloyl.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gtzzacvxos.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtnzriqabp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtpxusfnyk.html

PHP:  public / protected / private
来源：http://hz.jinghuilouyu.cn/gtmuigccwe.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtsidrwdsk.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtxwrbkzdz.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gttidmhkga.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtoinxodgo.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtwlteyhak.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gtdvdjblxt.html

[G11] getter / setter
来源：http://hz.ydzc1.top/gtfqowkthp.html

Py:   @property 与 @x.setter
来源：http://hz.jqgfzy.top/gtxfnterrk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtufomzdkx.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gtfxzoskpf.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtenvkcymu.html

Java: public String getName() { return name; }
来源：http://hz.sysykeji.top/gtvdmjuwna.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtrfpxzehp.html

Ruby: attr_accessor :name
来源：http://hz.dashuyun.cn/gtobtrhygk.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtckllbzbu.html

[G12] 对象转字符串
来源：http://hz.havefunace.top/gtdrvltyyv.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gtwokxntpm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtnnigurpk.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtblbrbuyl.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtznuqbfzq.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhengqikj.top/gtqphpacmu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gthzmvmuoo.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangtech.top/gtdtuwvsun.html

C#:   public override string ToString() => Name;
来源：http://hz.chenlongwang.top/gttlpexccb.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtapwqdclb.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangtech.top/gtimhwuheb.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtikzjxgbf.html

JS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtzkcmobqb.html

TS:   u instanceof User
来源：http://hz.jqgfzy.top/gteikpbkmz.html

Java: u instanceof User
来源：http://hz.cashguo.top/gtyuftmlhd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhongyouzk.top/gtfdqthtsa.html

Ruby: u.is_a?(User)
来源：http://hz.sufxvd.cn/gttjrwhxpo.html

C#:   u is User
来源：http://hz.fengsongda.top/gtphobpqrf.html

[G14] 数据类 / record
来源：http://hz.aibaodan.cn/gtfpoaipxl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gttanfncdp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gtpkqctlrd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuanzx.com/gthagpdbxb.html

TS:   type User = { name: string; age: number };
来源：http://hz.shzxlz.cn/gtowzhtgyb.html

Java: record User(String name, int age) {}
来源：http://hz.gzhubu.top/gtzryhvoux.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtqptwvaxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtqzblklgz.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtgmsfijzp.html

[G15] 枚举
来源：http://hz.guannengcc.top/gthcimbcmb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.quarkkingdee.top/gtdxwcdtqi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangshuangyany.cn/gtmffhumsy.html


<!-- 参考信息 -->