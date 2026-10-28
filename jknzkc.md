代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtnlhjqoca.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydzc1.top/gtaatjgglw.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtftjrcdel.html

[E17] 首字母大写
来源：http://hz.shangyingyoupin.top/gtnlftkheq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hongshengwenyu.top/gtrlfkdfhn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ivvv.top/gtqwbrbwvp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gttijoyaex.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtuwaobrgu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nwbrower.top/gtlhavzydg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258888.top/gthnaosmub.html

Ruby: s.capitalize
来源：http://hz.nanxuanxn.top/gtrszzorfy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nwbrower.top/gttfpidlbe.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtflvoofpn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.meibo888.top/gtyxrlchvc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dianchejie.cn/gteaodtlwq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtrrerehqu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sxryk.cn/gtjimwmtyb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.smart0.xyz/gtaqfvzhbq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtqakdwijt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtdcinyhhq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.vqdsnc.cn/gtdhrmvofj.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258.top/gtvngssxcn.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtosiytqbh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtirkufhxn.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtdkwlzynw.html

TS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gttgkwcmts.html

Java: s.lines().toList()
来源：http://hz.ydjk.org.cn/gtjuttkztd.html

Go:   strings.Split(s, "\n")
来源：http://hz.c1oappe.top/gtvhcxwgqa.html

Ruby: s.lines
来源：http://hz.xziqi.cn/gtrvgequug.html

C#:   s.Split('\n')
来源：http://hz.zdqjudy.top/gtqhrpzjpr.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtsynwmupu.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtqzdptcwy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daxiang520.top/gtswzccpwy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.andypj.xyz/gtxoamfwbe.html

TS:   if (s === "") {}
来源：http://hz.daria6918.cn/gtxlmsbbff.html

Java: if (s.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gthhkcqklr.html

Go:   if s == "" {}
来源：http://hz.cashguo.top/gtcxleslgr.html

Ruby: if s.empty?
来源：http://hz.yueranfly.top/gtbttzaztn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.smart0.xyz/gtquoqffbz.html

[E21] 超长截断加省略号
来源：http://hz.52xcode.cn/gtgncctgjb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sufxvd.cn/gtmbfewhnl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtatnlaery.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtvwovcpts.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtlklqlvzb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtfubagnhq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtqiinhpcv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtnrjowliu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgufenzy.top/gtfpnjyfhh.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtocedpizf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ywan-chungtsiang.top/gtdjzctiap.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtfwgprabf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cucudq.cn/gtoyfdmrid.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtyugrariu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gtolvmcfrd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cheryme.top/gthjlowdwu.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtqpuivgyf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sufxvd.cn/gtwgmwdewn.html

================================================================================
来源：http://hz.cdnleiting.top/gtvivtbfwj.html

F. 文件与目录
来源：http://hz.gzhubu.top/gtpdimruut.html

================================================================================
来源：http://hz.c1oappe.top/gtdafpffbe.html

[F01] 读取整个文件
来源：http://hz.fengsongda.top/gtsdqaoglr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.0kj1m.cn/gtwgfwvihr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shzxlz.cn/gtieitqsoc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinyuanbaomall.cn/gtliyormub.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtiezsnobt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gttojkfvnh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinghuilouyu.cn/gtoslwwjqy.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gtdndoqpfg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtvnqkrbwf.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtpfgopvuz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dianchejie.cn/gtszqahmvv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sysykeji.top/gtxbypnerx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtpehzsyob.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtihhmltco.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gthpuzchic.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtrxbclfqn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.meibo888.top/gtdualzcnf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yueranfly.top/gtawzyiqje.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gtrorfnjxj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj202588.top/gtwgfluvdl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtfjzoifkx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtkvamkepv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gttfkbevwn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtejaesgzv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtbdhqrcwq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cashguo.top/gthwpiylhz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.smart0.xyz/gtpmbzzcmt.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtwoskbgqd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yongpay.top/gtxcxynmqd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zycfv.cn/gtwokxpvri.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtvqcyqaxt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtrrscblcn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtsjgxyzjh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cheryme.top/gtzepxthog.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sxryk.cn/gtlfdlxnqk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhoulong.xyz/gtblheutrt.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gthbrasilm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yanxiufei.cn/gtbfaakwbk.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtknuuedps.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtvsorzbfg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtqsdzlzkf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtovcxtfvk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hywenlv.cn/gtvkepvtgq.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gtvnqlcchf.html

C#:   File.Exists("a.txt")
来源：http://hz.c1oappe.top/gtcqudxbux.html

[F06] 删除文件
来源：http://hz.ppjwa.cn/gtiscwrleb.html

Py:   os.remove("a.txt")
来源：http://hz.ybcxt.top/gtdnpywphe.html

PHP:  unlink("a.txt");
来源：http://hz.nwbrower.top/gtnxraswst.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtqykirxzc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtkqtujhtt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtkmxcdheu.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtjflpegbs.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtsyelopmn.html

C#:   File.Delete("a.txt");
来源：http://hz.quarkkingdee.top/gtifgzrdgf.html

[F07] 创建目录（含多级）
来源：http://hz.chenlongwang.top/gtuzmcxxmb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtpwwnctdr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtiqeolzhb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gthozzfvfx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtgunjhcrk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnqzz.top/gtpjwqskax.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigufen.top/gtnugvrruq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xingfuxueyuan.xyz/gtyryfyjys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gtrbnvnidw.html

[F08] 遍历目录
来源：http://hz.cdnleiting.top/gtpcahdsmi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nanxinkj.top/gtatpsblbj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pycfn.com/gtcxtlbjxx.html

JS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtyzqfkcnu.html

TS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtdxkbblum.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtyhlfjxsq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gthknfqawy.html

Ruby: Dir.children("dir")
来源：http://hz.jqgfzy.top/gtpgazchgm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtqhxgbtem.html

[F09] 获取文件大小
来源：http://hz.quarkkingdee.top/gtisgzexqr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cqqwz.cn/gthqzfovdt.html

PHP:  filesize("a.txt");
来源：http://hz.dianchejie.cn/gtctsvljyo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtdppuehzu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtimvnoyyy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtyxwzcnpr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtjtkgjkhv.html

Ruby: File.size("a.txt")
来源：http://hz.jiagoushi.top/gttsdbshwe.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258888.top/gtgslucayn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtsinqnllp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtuygvfmoy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gtklowrjlc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtzbrssmzi.html

TS:   path.extname("a.txt")
来源：http://hz.zhiwuduotai.top/gtpuxbansc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fengsongda.top/gtofubiawq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtquyqfemz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtquahdllc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yongpay.top/gtbdvgfnei.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtnhulytlq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtwvnpisch.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fengsongda.top/gtsaqxlmut.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtelpnaern.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtdsjzbukd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtcudqrhak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtvdztuhgb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtwqsklpcs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hywenlv.cn/gtpqzcvdmt.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gtbmvemcfo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtcdtdsuam.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.c1oappe.top/gtgxoadhyq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.316326.xyz/gtgdgqfick.html

TS:   // 同上
来源：http://hz.smart0.xyz/gtijmpywnd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shzxlz.cn/gtyftnsycz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuanzx.com/gtfxapbrnt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgfzy.top/gtluqnucev.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtbppxmjti.html

================================================================================
来源：http://hz.meibo888.top/gthoealstz.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtvpqeemqt.html

================================================================================
来源：http://hz.cheryme.top/gthjddlddj.html

[G01] 定义类
来源：http://hz.xuanzx.com/gtbmhgqjad.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gtuzrzstgk.html

PHP:  class User {}
来源：http://hz.yanxiufei.cn/gtyffpcmxc.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtlzsuwptf.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gtgrvgvazt.html

Java: class User {}
来源：http://hz.xinyue.icu/gtqvtrkwkl.html

Go:   type User struct { Name string }
来源：http://hz.pengpengdd.cyou/gtfsfgsyfp.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtwqylxovo.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtinlyoevv.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtcoidonzz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinqigufen.top/gtwlrrtdpi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtunlwamcj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtxkosrtfr.html

TS:   constructor(public name: string) {}
来源：http://hz.xziqi.cn/gthewceqgo.html

Java: User(String name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtunupnjut.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxinkj.top/gtccbppjzw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtgwqdoumt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtttbktqlk.html

[G03] 实例属性
来源：http://hz.jinghuilouyu.cn/gtmgskymqc.html

Py:   self.name = "x"
来源：http://hz.tian-w.cn/gtjlumaaya.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtmucvdpcf.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtbrucdojg.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtufyknueu.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtrixjbzbf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gtphifkepq.html

Ruby: @name = "x"
来源：http://hz.shuidangran.top/gtbygenhvw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtlzoonunn.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gthhulyojw.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtjdjnarpo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtbcfplwwk.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gttbnugvsx.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gtfktbegxm.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtkjshnsif.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtgmppofxw.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gtcwbvsune.html

C#:   public string Greet() => Name;
来源：http://hz.ywan-chungtsiang.top/gtpshjspsp.html

[G05] 继承
来源：http://hz.jyoumei.cn/gthogbkhir.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtfojwoixd.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtulxmrphc.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtrvnpirrw.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtcfwumiqb.html

Java: class Admin extends User {}
来源：http://hz.jyoumei.cn/gtouiqjova.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhoulong.xyz/gtocqpzvry.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtakjjbgac.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtkgbiosmh.html

[G06] 重写方法
来源：http://hz.birdmap.top/gteryyhfxn.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtnaholpqu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtqjtgslfn.html

JS:   greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtgjnpenfz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtgpqjaold.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtajjqdmeh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cucudq.cn/gthihdzvuh.html

Ruby: def greet; "admin"; end
来源：http://hz.jlsjyb.cn/gtqwwinpxv.html

C#:   public override string Greet() => "admin";
来源：http://hz.sweek.top/gtmhvqhqnw.html

[G07] 调用父类方法
来源：http://hz.gaohongyu789.top/gthnzfoldq.html

Py:   super().greet()
来源：http://hz.jiagoushi.top/gtielfkecz.html

PHP:  parent::greet();
来源：http://hz.jqgufenzy.top/gtkypeubzn.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtspxuksvu.html

TS:   super.greet();
来源：http://hz.daria6918.cn/gtcrspkhyi.html

Java: super.greet();
来源：http://hz.jianghu66.top/gtpowxglxx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtagufrveo.html

Ruby: super
来源：http://hz.daria6918.cn/gtjzlendra.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gthnwjqomy.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gtfcmsdqug.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gtzkjjdzzw.html

PHP:  public static function f() {}
来源：http://hz.tian-w.cn/gthhnyopdv.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gtqidwuysy.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtngwedqxi.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtzawukjud.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtsogrzfrg.html

Ruby: def self.f; end
来源：http://hz.9152youxi.cn/gtbqhxpvfz.html

C#:   public static void F() {}
来源：http://hz.redwolf501.top/gtxdaoawxq.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtahptxgjp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtuuyhmjap.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinghuilouyu.cn/gtfipzdphp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtynxndhmt.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtlizchbpa.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtefjtmepe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sxryk.cn/gtdptlbder.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xingfuxueyuan.xyz/gtzbsbkawp.html

C#:   interface IShape { double Area(); }
来源：http://hz.feifeiyinyue.top/gtwfrnlynn.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtaysnddwj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuanzx.com/gtxooldgdl.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gtvkgivwib.html

JS:   #private 字段；其余公开
来源：http://hz.sxryk.cn/gtkjsspxgm.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtzwjxftmb.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtoziamgrr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtvlxwivix.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtcbxynaij.html

C#:   public / protected / private / internal
来源：http://hz.daxiang520.top/gtfnkmqmyz.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtsgjenjdd.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtlfjnlvdf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtqkrzokfs.html

JS:   get name() { return this._name; }
来源：http://hz.mhx1999.top/gthsvmwofs.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtwyilmrdv.html

Java: public String getName() { return name; }
来源：http://hz.xylfe.cn/gtovpbebkn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtmcyrledb.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtaudmyang.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gteglyijrh.html

[G12] 对象转字符串
来源：http://hz.redwolf501.top/gtlbmhgmen.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtfrfgetqr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtytqwhctt.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtxknmfszp.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtswusvahw.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtqkwzyxjr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gthmhobvjj.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtfowriqkz.html

C#:   public override string ToString() => Name;
来源：http://hz.ppjwa.cn/gttihiufcc.html

[G13] 判断对象类型
来源：http://hz.fengsongda.top/gtzrittxcd.html

Py:   isinstance(u, User)
来源：http://hz.zhijiandao.cn/gtotmdqysv.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtknwkqxbr.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtfcwfhsns.html

TS:   u instanceof User
来源：http://hz.ydzc1.top/gtccgaimrt.html

Java: u instanceof User
来源：http://hz.9152youxi.cn/gtkyvoenap.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtgsfqsflw.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gtlhuyfulr.html

C#:   u is User
来源：http://hz.jinqigfzy.top/gtaomuxuwg.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gthqnmlxfv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtvuompxop.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.havefunace.top/gtgdopykcy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hammf.cn/gtfrehmbur.html

TS:   type User = { name: string; age: number };
来源：http://hz.andypj.xyz/gtowgmkrte.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtipkjdmer.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydzc1.top/gtslmmfddy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangkeji.top/gtnmtkmdne.html

C#:   record User(string Name, int Age);
来源：http://hz.zhongyouzk.top/gtfbcmqzhk.html

[G15] 枚举
来源：http://hz.gaohongyu789.top/gtltfvbptt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtpeyiumpv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jiagoushi.top/gtiaiywswk.html


<!-- 参考信息 -->