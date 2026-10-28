代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tian-w.cn/gtigtwvbww.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gteqflybyg.html

C#:   1234567.ToString("N0")
来源：http://hz.aizwys.cn/gtforwscml.html

[E17] 首字母大写
来源：http://hz.ydjk.org.cn/gtwqlooujm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ppjwa.cn/gtvfcksfaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gtkbaaijkd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gttnjsjmdy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtacoobpfs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xziqi.cn/gtlivzvfyh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.9152youxi.cn/gtcuehgram.html

Ruby: s.capitalize
来源：http://hz.ybcxt.top/gtgndffpnt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtpewhpelf.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtakymmmig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtobslxfbh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cucudq.cn/gtcfmuthuf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtahhkrifa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtzaktvdxl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtxcdxvivz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gtqnmveuxj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangtech.top/gtswourvpa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhixingplan.top/gtnyahzvat.html

[E19] 多行文本按行拆分
来源：http://hz.nanxinkj.top/gtyizbuqnw.html

Py:   s.splitlines()
来源：http://hz.ywan-chungtsiang.top/gtklpikswg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhixingplan.top/gtdshthhvb.html

JS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtlxjfxlvh.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtfqrqgfkx.html

Java: s.lines().toList()
来源：http://hz.dianchejie.cn/gtvgklaqrv.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtxzizqxoj.html

Ruby: s.lines
来源：http://hz.nwbrower.top/gtowgvtgvu.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtyubpgype.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gtqroxrxgq.html

Py:   if not s:
来源：http://hz.ydzc1.top/gtfwlidqyn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pengpengdd.cyou/gtyvmhptit.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ppjwa.cn/gtozmsndcb.html

TS:   if (s === "") {}
来源：http://hz.jyoumei.cn/gtskjdazsa.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtarpcwfsc.html

Go:   if s == "" {}
来源：http://hz.zhaomingkeji.xyz/gtliubfcku.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gtxqeisdpz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtikqstfur.html

[E21] 超长截断加省略号
来源：http://hz.iojbl.cn/gtiohcnjrr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gtjcqoglaa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtqqikcutl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtxbdaoihb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtjtewxapv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtbyzonkpi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtxbbszegk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cdnleiting.top/gtwzuypkmr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sysykeji.top/gtpfgcwopj.html

[E22] 字节长度与字符长度
来源：http://hz.sysykeji.top/gtkkyooanl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gtlrjrahzy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtjhyceqtg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtskhcbmao.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtfsifrzbt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtfuzbbqxx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shangyingyoupin.top/gtjhbajtuq.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtsjcqjace.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gotoacloud.top/gtmthpmbez.html

================================================================================
来源：http://hz.chenzaomai.com/gtxrdaejdw.html

F. 文件与目录
来源：http://hz.tianlin.xyz/gthmylteqf.html

================================================================================
来源：http://hz.tianlin.xyz/gtkijcxecw.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtlxyiyrjn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtpguayuwf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gtbopeysbb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinyuanbaomall.cn/gtzqanqihs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gthtxxlfdk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtlltpdfav.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenlongwang.top/gtyyspvdme.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtnxepfrqd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cucudq.cn/gtvarccgov.html

[F02] 逐行读取文件
来源：http://hz.tian-w.cn/gtbknzlljy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtgqmxdszn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenlongwang.top/gtpcdbsejw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtsirddahi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtedvdlnff.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtpznqfncm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nwbrower.top/gtaymeydob.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.bjfxy.top/gtofbsvzsm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtfujqveph.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtlwstlfkd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinyuanbaomall.cn/gtihogsqmx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtusbrqhnr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtpqckkeew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtgqquveuv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtujgrgcfc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtyrgtwzwn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtjxdgwjqn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gthwmolimq.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtsokxnszc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtfejizzym.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuanzhike.top/gtfzrxjutx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gthzibeyrx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtztzfhwef.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gtjidttynu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtkellsmru.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.vqdsnc.cn/gtjruubnds.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtllcrsnwn.html

[F05] 判断文件或目录是否存在
来源：http://hz.52xcode.cn/gtfwoxwsls.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ivvv.top/gtkcprwqtx.html

PHP:  file_exists("a.txt");
来源：http://hz.haohaochexian.top/gtmtwfibyt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtgaatvftn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtqgtpakjo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtdxotgppv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yanxiufei.cn/gtzunnzajo.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtxkdfgtlz.html

C#:   File.Exists("a.txt")
来源：http://hz.52xcode.cn/gtakzodqko.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtdtklyhdg.html

Py:   os.remove("a.txt")
来源：http://hz.yj202588.top/gtngvkgmzg.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gtefhmfcgl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtaoczeoju.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jlsjyb.cn/gtujrzqgwa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtjldmufqm.html

Go:   os.Remove("a.txt")
来源：http://hz.cqqwz.cn/gtulvzsbjk.html

Ruby: File.delete("a.txt")
来源：http://hz.mhx1999.top/gtgnooudsz.html

C#:   File.Delete("a.txt");
来源：http://hz.c1oappe.top/gtemzwacxb.html

[F07] 创建目录（含多级）
来源：http://hz.xuanzx.com/gtpfzqycqs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtuzscsplq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtfrpehzer.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtoxrwfkam.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtthmbsecf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj202588.top/gteutfvpro.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pycfn.com/gtykaxyjpv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.c1oappe.top/gtjjjqxasf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtbrzwywfs.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gtrrcqzsda.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtdcsmgylu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gtzxridksh.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtqqbwfspn.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtifitdljx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtfvcwkpfw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gotoacloud.top/gtykcqkpmk.html

Ruby: Dir.children("dir")
来源：http://hz.jianghu66.top/gtkchpzkhn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yongpay.top/gtfgfbkcpe.html

[F09] 获取文件大小
来源：http://hz.jinqigfzy.top/gtuzmnkusz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtuigkeenf.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gttwapkggy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtyxzhivnb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtizknodmx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtzdfndtkc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtlkhtstso.html

Ruby: File.size("a.txt")
来源：http://hz.xuanzx.com/gtirjafids.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.svipenyu.cn/gtabatlvrc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jlsjyb.cn/gtfnjabync.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtmfuaktdz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ivvv.top/gtqbqnfcpj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtfwcvrmiw.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtgozuzbhk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxinkj.top/gtidszmhoz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cheryme.top/gtuocynthk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtgbnjjctz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigufen.top/gtaxqkuqgd.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtbokxdirg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtwjfqxmbn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigfzy.top/gtzpactneg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gthamzwmrc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtvtbyseus.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fzhhl.top/gtgdmwjzch.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gttrjfgaix.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gteazbuqcc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtwordxzhx.html

[F12] CSV 读写
来源：http://hz.shuidangran.top/gtwennjhqx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gtifntxeuh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtziynwgsd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtutgcrkvo.html

TS:   // 同上
来源：http://hz.yueranfly.top/gtdimjgvdk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gzhubu.top/gttbgnbams.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtjinicpwm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gtjbmfsymp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gtdhnvsatd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwxxuzpxn.html

G. 面向对象
来源：http://hz.yongpay.top/gtpltnampv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmwhinxxs.html

[G01] 定义类
来源：http://hz.jinyuanbaomall.cn/gtqiceudtv.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtwnjsgyci.html

PHP:  class User {}
来源：http://hz.sxryk.cn/gtamodlzva.html

JS:   class User {}
来源：http://hz.316326.xyz/gtngbquupg.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtcszhvxqk.html

Java: class User {}
来源：http://hz.ydzc1.top/gtuusizblp.html

Go:   type User struct { Name string }
来源：http://hz.jinqigfzy.top/gtpjuupvxx.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtqxqoytyf.html

C#:   class User {}
来源：http://hz.guowangkeji.top/gtuugyjzck.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtuwfuwqoe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtzduqlcna.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gogol.net.cn/gtkmspdunn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtnidydmag.html

TS:   constructor(public name: string) {}
来源：http://hz.gotoacloud.top/gtwtaqyjox.html

Java: User(String name) { this.name = name; }
来源：http://hz.yueranfly.top/gtoqkutbnp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gttebmslmw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtycaccyjr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gthfawhhus.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtjttiolbv.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtqyaqitrt.html

PHP:  public string $name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtqhwanoug.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtjttlqbhy.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtljeulotg.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtnsysrddk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gttxrkfrdv.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtmbacnzqw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.c1oappe.top/gtxbyzyxah.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtswgjynlk.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gtepdinbvu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtigptgtrn.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtgcdihbal.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtictlhutt.html

Java: String greet() { return name; }
来源：http://hz.tianlin.xyz/gttjvjhcqt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtvqhjcihm.html

Ruby: def greet; @name; end
来源：http://hz.c1oappe.top/gtntyokqyp.html

C#:   public string Greet() => Name;
来源：http://hz.yj202588.top/gtuvvpunce.html

[G05] 继承
来源：http://hz.sweek.top/gtgrrkzzpy.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtmouynnkb.html

PHP:  class Admin extends User {}
来源：http://hz.ydzc1.top/gtlliwwaeq.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtvhgchzok.html

TS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gttqqejsyh.html

Java: class Admin extends User {}
来源：http://hz.yj202588.top/gtwkariitf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtilqvmksu.html

Ruby: class Admin < User; end
来源：http://hz.birdmap.top/gtdnakmrwn.html

C#:   class Admin : User {}
来源：http://hz.jqgufenzy.top/gtycajrstx.html

[G06] 重写方法
来源：http://hz.snrcjt.cn/gtjlcnvikl.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtzdwhiruj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtbiqpdadt.html

JS:   greet() { return "admin"; }
来源：http://hz.tanke756.top/gttiodhsvn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtpkzypfit.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtpxfhbpce.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenlongwang.top/gtpuupsurt.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtiveywuaj.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtfgkhpyjl.html

[G07] 调用父类方法
来源：http://hz.zhoulong.xyz/gtisoaroyz.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtvlnkwrrj.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gttaepkhdy.html

JS:   super.greet();
来源：http://hz.gogol.net.cn/gtkecnlgoh.html

TS:   super.greet();
来源：http://hz.ppjwa.cn/gtpgevvfus.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gttyvydfsp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtjirofqmc.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gtjbyrdmhu.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gtyexwejkr.html

[G08] 静态方法与属性
来源：http://hz.pengpengdd.cyou/gtujftworb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtbuwbnivq.html

PHP:  public static function f() {}
来源：http://hz.zdqjudy.top/gtzuywunhj.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtaebpahxw.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtyseloxin.html

Java: static void f() {}
来源：http://hz.jinyuanbaomall.cn/gtmhmvwgus.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuetiantiany.cn/gtazlwhoyj.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtlsnkhnno.html

C#:   public static void F() {}
来源：http://hz.jiagoushi.top/gtjgergibw.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gttxnbxcns.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gtsebuztfr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtqdqzbhuj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cucudq.cn/gtdgcnocwj.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtiflnobhw.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtpnqhacmx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tianlin.xyz/gtvcvlwlxc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj202588.top/gtzebattvp.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtlxkjnvad.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtsyreiidm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.feifeiyinyue.top/gteogwydnb.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtfqbqnqel.html

JS:   #private 字段；其余公开
来源：http://hz.hnqzz.top/gttrvyyhui.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtmduzknhh.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtngoqvrrv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xylfe.cn/gtzxbjguwj.html

Ruby: public / protected / private
来源：http://hz.hongshengwenyu.top/gtzlunfehb.html

C#:   public / protected / private / internal
来源：http://hz.redwolf501.top/gtncvqppdp.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtrkfhpypi.html

Py:   @property 与 @x.setter
来源：http://hz.nanxinkj.top/gtjfjupjcf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtqwbolhxq.html

JS:   get name() { return this._name; }
来源：http://hz.cashguo.top/gtqkxajkox.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gtkricevgm.html

Java: public String getName() { return name; }
来源：http://hz.snrcjt.cn/gtseyqazwq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.52xcode.cn/gtmhwnqunn.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangkeji.top/gtgjctuukj.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtzhyciehi.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtoyjipbhy.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtxdqcooen.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.mhx1999.top/gthjrrxagl.html

JS:   toString() { return this.name; }
来源：http://hz.vqdsnc.cn/gtqkcloivm.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtlmuojkud.html

Java: @Override public String toString() { return name; }
来源：http://hz.daxiang520.top/gtamoetqnf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtcmptoqbh.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gtvnmxmsnx.html

C#:   public override string ToString() => Name;
来源：http://hz.zdqjudy.top/gtwgpwigev.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gtutofxolr.html

Py:   isinstance(u, User)
来源：http://hz.yj202588.top/gthzxjdaoz.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtejzqodkl.html

JS:   u instanceof User
来源：http://hz.chenzaomai.com/gtasvkkoym.html

TS:   u instanceof User
来源：http://hz.hnqzz.top/gtukkzadci.html

Java: u instanceof User
来源：http://hz.pycfn.com/gtzwmbdizx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.meibo888.top/gtrlqrqixm.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtlagcetwf.html

C#:   u is User
来源：http://hz.zdqjudy.top/gtlhxvihko.html

[G14] 数据类 / record
来源：http://hz.ehwqpu.com/gtjejxfolr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aibaodan.cn/gtguclttsh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtkptwythj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yvedp.cn/gtbzyfbvtn.html

TS:   type User = { name: string; age: number };
来源：http://hz.haohaochexian.top/gthdcgavjp.html

Java: record User(String name, int age) {}
来源：http://hz.hnxiangtu.top/gtwkzwcqnf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gttorookfy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gaohongyu789.top/gtvkzowlax.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtedpzfshh.html

[G15] 枚举
来源：http://hz.zdqjudy.top/gtvswuryza.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtdefhtkda.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.bjfxy.top/gtpgnkjvqy.html


<!-- 参考信息 -->