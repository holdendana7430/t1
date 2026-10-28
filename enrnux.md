代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hfpthk.cn/gtgsemdofj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhengqikj.top/gtudcehopi.html

[E16] 数字千分位
来源：http://hz.jiagoushi.top/gtbuixkiwq.html

Py:   f"{1234567:,}"
来源：http://hz.hywenlv.cn/gtxsznrnsl.html

PHP:  number_format(1234567);
来源：http://hz.shzxlz.cn/gtjxwqvttc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtcxrouybr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtvwrlblws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daxiang520.top/gtjijmphkc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.feifeiyinyue.top/gtrfknfkcc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gzhubu.top/gtrpfrqbmn.html

C#:   1234567.ToString("N0")
来源：http://hz.ywan-chungtsiang.top/gturclporg.html

[E17] 首字母大写
来源：http://hz.guannengcc.top/gtbqjlkboz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtfmiirqmq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenzaomai.com/gtsvbxreqc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtragspryv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtkgcfemhd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xinyue.icu/gtunhmbvid.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cheryme.top/gtnmsbvudy.html

Ruby: s.capitalize
来源：http://hz.sysykeji.top/gtskttweun.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtnjzqhrat.html

[E18] 模板占位符替换
来源：http://hz.316326.xyz/gtlgnzxhqk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gtpithevhu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aizwys.cn/gtngizuxze.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtftgdydwh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtvqdboaco.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258.top/gtifsysums.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tanke756.top/gtvjgvbusb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gotoacloud.top/gtbimjtngu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnxiangtu.top/gticdeidwg.html

[E19] 多行文本按行拆分
来源：http://hz.mhx1999.top/gtfstgtehx.html

Py:   s.splitlines()
来源：http://hz.ydzc1.top/gtxmuvtdbh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxinkj.top/gtcscfohlg.html

JS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtsvnrqgwg.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gthoevryme.html

Java: s.lines().toList()
来源：http://hz.snrcjt.cn/gthdqdxfok.html

Go:   strings.Split(s, "\n")
来源：http://hz.ppjwa.cn/gtqfkncgxe.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtddeqabor.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtkxfejjwr.html

[E20] 判断字符串是否为空
来源：http://hz.shuidangran.top/gtyjtcxdsn.html

Py:   if not s:
来源：http://hz.cheryme.top/gtagkvpexb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtcgwtjxkd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.quarkkingdee.top/gtixpejvfz.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gtohqanxfr.html

Java: if (s.isEmpty()) {}
来源：http://hz.andypj.xyz/gtuntxwing.html

Go:   if s == "" {}
来源：http://hz.yuxming.cn/gtkpgqwbqc.html

Ruby: if s.empty?
来源：http://hz.ydjk.org.cn/gttumzlzjy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtmkhjicii.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtnfygamle.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yvedp.cn/gtmdzaejxx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtohtyafoz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtgcgphgup.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtojpkhbsl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtinpnyvaq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtgenpusmo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pycfn.com/gtugslujcb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yanxiufei.cn/gtmmnvrkdd.html

[E22] 字节长度与字符长度
来源：http://hz.hysaishi.cn/gtqfbvyngm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuanzhike.top/gtbmtgasve.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtiilpqurb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gtmxbkhrjp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtyxkzxqhj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yueranfly.top/gtezlcauik.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dianchejie.cn/gtzgcyoyaq.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtptsjiuuy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shzxlz.cn/gtwuxpktrx.html

================================================================================
来源：http://hz.meibo888.top/gturcmwtin.html

F. 文件与目录
来源：http://hz.shuidangran.top/gtoibtzcdi.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbggvadqk.html

[F01] 读取整个文件
来源：http://hz.xinyue.icu/gtszevnsii.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.quarkkingdee.top/gtypobiryu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtdipvxdfi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hysaishi.cn/gtbpmsqoel.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtcfezldpa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtihgvnmem.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ppjwa.cn/gtrsfbwgzp.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtpgwnpioz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tian-w.cn/gtuhtfpmuw.html

[F02] 逐行读取文件
来源：http://hz.zhengqikj.top/gtkblfquxc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tanke756.top/gtagytudqb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtnqtatvla.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtyxbsurxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gthvhlsvye.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtffwjmpml.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhaomingkeji.xyz/gtfyyufgxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuxming.cn/gtbjhgwkxy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenjidiqi.icu/gtgibwostf.html

[F03] 写入文件（覆盖）
来源：http://hz.zhijiandao.cn/gtzcnkzioh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtsspbhfeh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtbgyotszp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtnisnlqoa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gthcbkwjgg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.kuanghao11.cn/gttrmrsdkp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zycfv.cn/gtxusrlnzh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenzaomai.com/gtrkzjmosr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xinyue.icu/gtpfbutcri.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtplkfnvjx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangkeji.top/gtvremvzyb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sweek.top/gtexoktwky.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtlluvonsx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtzimgtseo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtsuqoopic.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigfzy.top/gtyhlodktm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gtptqnkqef.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zdqjudy.top/gtdhylypae.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtvnwonadk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtzdjutpzx.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtpudsaoif.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtlgkgddyb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtvyuejceu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtbzdivhvs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nwbrower.top/gtdzxyptzp.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtyxjssnuh.html

C#:   File.Exists("a.txt")
来源：http://hz.zhongyouzk.top/gtgpiefovi.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtkszvzaqd.html

Py:   os.remove("a.txt")
来源：http://hz.mhx1999.top/gtkczdftxr.html

PHP:  unlink("a.txt");
来源：http://hz.xziqi.cn/gtjugctbgn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtddqeygwk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtorybenkn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtbbsiztrf.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtclnvyhzc.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtoafacyiv.html

C#:   File.Delete("a.txt");
来源：http://hz.jinghuilouyu.cn/gturnodnyg.html

[F07] 创建目录（含多级）
来源：http://hz.pycfn.com/gtojuzfwfj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hysaishi.cn/gtewkoicsz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.svipenyu.cn/gtfsjbkkvn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aizwys.cn/gtoaytczim.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtltlyioxn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtzkxrnxng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtfltxgzwu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtkwfdoywa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cashguo.top/gtejrwidyd.html

[F08] 遍历目录
来源：http://hz.yj20258.top/gtwhlrcwnb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydzc1.top/gtateeaake.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jianghu66.top/gtdffxeeva.html

JS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtyiwpdxlx.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtbrdjycwm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtonhudrta.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yonumen.top/gtjslgrgwg.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gtjhbnwypr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtwiwlsygm.html

[F09] 获取文件大小
来源：http://hz.zhiwuduotai.top/gtmqlwlxiu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cheryme.top/gtrzjwkqmg.html

PHP:  filesize("a.txt");
来源：http://hz.dashuyun.cn/gtrmmatprz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtodymprpl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtgzhdgplp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtqqcvypbl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fzhhl.top/gtgzaugtxr.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gtymrklfwq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dianchejie.cn/gtwxyfpelm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtvdijvyix.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtfujluusb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.smart0.xyz/gtknfkdoem.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtwtnqxlwr.html

TS:   path.extname("a.txt")
来源：http://hz.tianlin.xyz/gtqzirpklx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shzxlz.cn/gtnkapypfd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtqvnmuelk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtowfkrmhu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtvfgghfyx.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtdmohqhlq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gttwmvqexp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aizwys.cn/gtajjpvzas.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtizwqbepl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtrlcfumpl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hongshengwenyu.top/gtdbbdqqen.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuetiantiany.cn/gtxgipwass.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtsuhuueav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gzhubu.top/gttdpyfgdu.html

[F12] CSV 读写
来源：http://hz.hongshengwenyu.top/gtilccpfjt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gthwvdijgz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtikwkclby.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shzxlz.cn/gtxrklpxvs.html

TS:   // 同上
来源：http://hz.aizwys.cn/gtgcwdjnae.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtuexmiqhy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gtwuotemxt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtyyxyrrnf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtcmyhhmzy.html

================================================================================
来源：http://hz.xuanzx.com/gtxocopfwu.html

G. 面向对象
来源：http://hz.wangdashe.top/gtfjmbmnju.html

================================================================================
来源：http://hz.sxryk.cn/gtvsbmjybx.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtgcmdoduo.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtqkinrwmq.html

PHP:  class User {}
来源：http://hz.yonumen.top/gtmlnzfang.html

JS:   class User {}
来源：http://hz.ydzc1.top/gtxtzpxghq.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtwqfpotmx.html

Java: class User {}
来源：http://hz.hnqzz.top/gtcxgjfaax.html

Go:   type User struct { Name string }
来源：http://hz.tian-w.cn/gtynhbhchd.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtwpkhkbiv.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtuxnnmayy.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gtlglwjmdl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtnjmwmlto.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtuhssiwuw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtthbdmlgy.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtuqpginpr.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gtwgsowpvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtggjklwaa.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtoxmnvdgk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.316326.xyz/gtzxzgkqko.html

[G03] 实例属性
来源：http://hz.hnqzz.top/gtctjgqeue.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtofkmlpab.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtbelfxpph.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtgewzqvcp.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtvgvnsrgy.html

Java: private String name;
来源：http://hz.nwbrower.top/gtzbvtsgad.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daxiang520.top/gtjzhahawr.html

Ruby: @name = "x"
来源：http://hz.hfpthk.cn/gtnesedvst.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.feifeiyinyue.top/gtevxroacj.html

[G04] 定义方法
来源：http://hz.yvedp.cn/gtsfpaspmr.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gtpblsvdzq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtwysdghus.html

JS:   greet() { return this.name; }
来源：http://hz.havefunace.top/gtyetagffc.html

TS:   greet(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtnsfddvtc.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gtsdflksjn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtgutneqpu.html

Ruby: def greet; @name; end
来源：http://hz.birdmap.top/gtarqtzfce.html

C#:   public string Greet() => Name;
来源：http://hz.xinyue.icu/gtzsikcxwt.html

[G05] 继承
来源：http://hz.zhiwuduotai.top/gtvegoeqej.html

Py:   class Admin(User): pass
来源：http://hz.9152youxi.cn/gttdesuqfn.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258.top/gtlpcbxzai.html

JS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtquxbkyjf.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtmbwlmibm.html

Java: class Admin extends User {}
来源：http://hz.52xcode.cn/gtpftfoiqv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.birdmap.top/gttdfaaybm.html

Ruby: class Admin < User; end
来源：http://hz.dianchejie.cn/gtxhmkhdtf.html

C#:   class Admin : User {}
来源：http://hz.zhijiandao.cn/gtjlxtrjlt.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtosjpdexa.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtdavotniv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtdnypjqwc.html

JS:   greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtceehbgct.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtenaguctm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtvqchfhjq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtzetmmoiu.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtppvzlobk.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtoocabejo.html

[G07] 调用父类方法
来源：http://hz.yj20258.top/gtvumktrgq.html

Py:   super().greet()
来源：http://hz.zhengqikj.top/gtfmgkwtgc.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtvnnilwqy.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtihmbykxs.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtsfldqxrc.html

Java: super.greet();
来源：http://hz.smart0.xyz/gtkfobpicj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gttvluloib.html

Ruby: super
来源：http://hz.bjfxy.top/gtjnyezfek.html

C#:   base.Greet();
来源：http://hz.yuanzhike.top/gtualjqejz.html

[G08] 静态方法与属性
来源：http://hz.birdmap.top/gtfwxaolih.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangtech.top/gtihssrqoo.html

PHP:  public static function f() {}
来源：http://hz.birdmap.top/gtwkflxuxv.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtpylnaane.html

TS:   static f(): void {}
来源：http://hz.hnqzz.top/gtkgegzxch.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtlgcttvvn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.52xcode.cn/gtdersydcf.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtdhwpxwpu.html

C#:   public static void F() {}
来源：http://hz.pengpengdd.cyou/gtwtxpuvyi.html

[G09] 接口 / 抽象类
来源：http://hz.hammf.cn/gtwvujggqk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtiadpckai.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtmzajvzxy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtpqfdktnv.html

TS:   interface Shape { area(): number; }
来源：http://hz.havefunace.top/gtbikgaxgc.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtrcssvdwj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtlvhmlgvj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gogol.net.cn/gtnkmkhhfg.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtrbovyghy.html

[G10] 访问控制
来源：http://hz.jinqigufen.top/gtykgcfyfz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gteqxintzp.html

PHP:  public / protected / private
来源：http://hz.sxryk.cn/gthwmbppzv.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtbfbwngjg.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtiqkidugi.html

Java: public / protected / private / 默认包级
来源：http://hz.cheryme.top/gtrqvmvocd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtvutrssao.html

Ruby: public / protected / private
来源：http://hz.316326.xyz/gtfggbfuau.html

C#:   public / protected / private / internal
来源：http://hz.chenlongwang.top/gtetjgpsvx.html

[G11] getter / setter
来源：http://hz.jianghu66.top/gtspaxeauk.html

Py:   @property 与 @x.setter
来源：http://hz.fengsongda.top/gtfnzcnfce.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtxyejvolo.html

JS:   get name() { return this._name; }
来源：http://hz.yvedp.cn/gtcbqqqqez.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxinkj.top/gtacpffamg.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtimnndcgq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daxiang520.top/gttvwhfuya.html

Ruby: attr_accessor :name
来源：http://hz.zhixingplan.top/gtvmwfvbuo.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtgjqibwfk.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gtnfwofcge.html

Py:   def __str__(self): return self.name
来源：http://hz.yongpay.top/gtzebzimwy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtcxnhhdyu.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258.top/gtlzfqvgaf.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtwtmfzvoz.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtbrmmvwme.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtxgdwqqzx.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtequyjxqa.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtnrscmkkx.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtkdbxwgkn.html

Py:   isinstance(u, User)
来源：http://hz.sysykeji.top/gtmdeippdt.html

PHP:  $u instanceof User
来源：http://hz.kuanghao11.cn/gtnjadhsmw.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gteseskwwp.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gtkandpgkk.html

Java: u instanceof User
来源：http://hz.dianchejie.cn/gtwknltyjm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtgaqluqag.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigfzy.top/gtfdkqthhc.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtudoswqbq.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtipdxcurw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gtucnjmdwx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guowangkeji.top/gteunjccjh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtvrggyszh.html


<!-- 参考信息 -->