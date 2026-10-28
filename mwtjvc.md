代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.gaohongyu789.top/gtubwstjyp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtitrqpzxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gtcxnraukq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yongpay.top/gtvvgfqota.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangtech.top/gtyyeikpoj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.316326.xyz/gtkmhjdmiv.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gtbohjqblr.html

[E17] 首字母大写
来源：http://hz.yj202588.top/gtlnqjfwnz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtxuqwtaon.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pengpengdd.cyou/gtpycxdmzv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtrcalgvhz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtllncpdof.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuanzx.com/gtebmfrzik.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhoulong.xyz/gtqinqhtqf.html

Ruby: s.capitalize
来源：http://hz.jiagoushi.top/gtgsehzzzg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sysykeji.top/gtqzzunfqh.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtammhkbhk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.meibo888.top/gtpuziyroh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xziqi.cn/gtlftgynnc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtvtkguubi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtvzbzmrbm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.birdmap.top/gtvxupuaqb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gtjisywkaa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jianghu66.top/gtzicpbodu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jiagoushi.top/gtqvosydwr.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtwkfwexlh.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangtech.top/gtiazozlbt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xziqi.cn/gtiwbmqbth.html

JS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtnrrqpuhk.html

TS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtedupbfjj.html

Java: s.lines().toList()
来源：http://hz.yonumen.top/gtdodwfxaa.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gttxqpmwbu.html

Ruby: s.lines
来源：http://hz.tanke756.top/gtmsppqisw.html

C#:   s.Split('\n')
来源：http://hz.316326.xyz/gtrghaqotw.html

[E20] 判断字符串是否为空
来源：http://hz.pengpengdd.cyou/gtavripafz.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtlgrkbjgj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtvdkxkbbr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtnkwbaknq.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gterwdddpg.html

Java: if (s.isEmpty()) {}
来源：http://hz.yvedp.cn/gtnbbdvnlu.html

Go:   if s == "" {}
来源：http://hz.daria6918.cn/gtoeurcftq.html

Ruby: if s.empty?
来源：http://hz.meibo888.top/gtybayjhta.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gtpzttzvtc.html

[E21] 超长截断加省略号
来源：http://hz.chenzaomai.com/gtszvohokp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenzaomai.com/gtscueteix.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenjidiqi.icu/gtrslrkmje.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtrwfcznpd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtogtnyqid.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtehclpdkw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hammf.cn/gtnuuiqcrr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gtzotynzcr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhoulong.xyz/gteagclvoy.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gtcyzleyyi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtacqkupvs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gteqisjori.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtdqaqrvig.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtucswcceg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhengqikj.top/gtqbeceueg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtyarwzueo.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtftkttfzj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.svipenyu.cn/gtxzsjxgza.html

================================================================================
来源：http://hz.zhijiandao.cn/gtotcbasgg.html

F. 文件与目录
来源：http://hz.shuidangran.top/gtbnvgqdcm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkpzcbyyj.html

[F01] 读取整个文件
来源：http://hz.9152youxi.cn/gtflawxxck.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gaohongyu789.top/gtquwnzdco.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtykgjqqxl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtzdecbegn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxuanxn.top/gtogdjlzuf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtxbpwguge.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ydzc1.top/gtsxwgipzj.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtcxlxrnbz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guannengcc.top/gtxnjmjuys.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gthnjwikwk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gotoacloud.top/gtwdshndml.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gtovzrkaqj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtrczyeicw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtzekudxvn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtubdpfnzy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sweek.top/gtgdaiemve.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtpwqqjbme.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.iojbl.cn/gtlhgjfbae.html

[F03] 写入文件（覆盖）
来源：http://hz.aizwys.cn/gtqnxhbmxc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hysaishi.cn/gteotptxyk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtsygpdhur.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtcoxyipop.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtqxvptocx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gaohongyu789.top/gtaucjoxbr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.snrcjt.cn/gtgyarrkml.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tian-w.cn/gtsdktfhrl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.316326.xyz/gtdypajeaq.html

[F04] 追加写入文件
来源：http://hz.tianlin.xyz/gteadmsyfo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydzc1.top/gtipgqtqrd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.vqdsnc.cn/gtplluljit.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtdavrqhbj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtsidxepvf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtyyyalchu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtrybvpret.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gthxcakcip.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtqvngduwh.html

[F05] 判断文件或目录是否存在
来源：http://hz.0kj1m.cn/gttmsrkkaj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yanxiufei.cn/gthvqcymaf.html

PHP:  file_exists("a.txt");
来源：http://hz.cqqwz.cn/gtfbtoxtui.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtfwvraxlo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtxcsughbk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gttxgtgxlw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sysykeji.top/gtobqjbdqz.html

Ruby: File.exist?("a.txt")
来源：http://hz.cashguo.top/gtmhjkqrnj.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtljsnueku.html

[F06] 删除文件
来源：http://hz.yonumen.top/gtgtvhmzpt.html

Py:   os.remove("a.txt")
来源：http://hz.yuanzhike.top/gtniipunny.html

PHP:  unlink("a.txt");
来源：http://hz.cdnleiting.top/gtgbtsjpwb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtwxvrxefr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtvnnjynrg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtfeqhjlsk.html

Go:   os.Remove("a.txt")
来源：http://hz.yuxming.cn/gtcsbwhnlu.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtmahfbnbh.html

C#:   File.Delete("a.txt");
来源：http://hz.sweek.top/gtbdbmjjay.html

[F07] 创建目录（含多级）
来源：http://hz.yuxming.cn/gtdgbnxzbc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gtfnavxlec.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shuidangran.top/gtpbkktyii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtzawaaqwa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtzgetwbve.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daxiang520.top/gtsmsrxsrd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gtgrjcxmfw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.feifeiyinyue.top/gtfbjxdutz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtyrsdupmx.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtpehhzpao.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.vqdsnc.cn/gtmbvriuid.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ehwqpu.com/gtwnylpqmg.html

JS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtlvwfbiei.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhongyouzk.top/gtzomfbezt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtmjfiahgk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtlqjcyvqi.html

Ruby: Dir.children("dir")
来源：http://hz.yangfankeji.com/gtlsdulbuu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtfisdmfct.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtxghshpun.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fzhhl.top/gtqviiagns.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtxrvegaee.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtgykyronh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtoxjjqhlr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtmggxynzc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtfczvqmit.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtinmjpeys.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tanke756.top/gtoywrmyyv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtaxxqxfnz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtqethuehe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtrdvqvsow.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gthffdxkrc.html

TS:   path.extname("a.txt")
来源：http://hz.cqqwz.cn/gtllfrchxd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhiwuduotai.top/gtzjnpgiqn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtkievbdew.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtsjcdrbbq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtvnsnfzad.html

[F11] 复制与移动文件
来源：http://hz.gaohongyu789.top/gtzwusddks.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtehajhtza.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.iojbl.cn/gtrktkfgsw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtedaldzac.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtryewiqqv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gtsnvblzfx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cashguo.top/gtnyphsmgx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtonqejdrl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cucudq.cn/gtpjzxrwne.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gtrthvxkqi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtyqoyjhhh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhiwuduotai.top/gtirefbofq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jyoumei.cn/gtwwdwugtu.html

TS:   // 同上
来源：http://hz.yonumen.top/gtjxwazghi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gtttrzaqme.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtjueomxxf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuanzx.com/gtzynfjikg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xylfe.cn/gtrkihqwrr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzvlaizzi.html

G. 面向对象
来源：http://hz.ydzc1.top/gteakiyspr.html

================================================================================
来源：http://hz.haohaochexian.top/gtpnwwutjm.html

[G01] 定义类
来源：http://hz.birdmap.top/gtmdxywijr.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtwtcvxcxu.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtbwuqacfw.html

JS:   class User {}
来源：http://hz.ydjk.org.cn/gtomtgqscc.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtciixsuic.html

Java: class User {}
来源：http://hz.daxiang520.top/gtccolqcmz.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gthdiyevcq.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtfsiiibcy.html

C#:   class User {}
来源：http://hz.jyoumei.cn/gtukbayxbs.html

[G02] 构造函数
来源：http://hz.0kj1m.cn/gtgbwedceg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnxiangtu.top/gtflomdenk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daria6918.cn/gtxckcinvp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.havefunace.top/gtcddpfxqz.html

TS:   constructor(public name: string) {}
来源：http://hz.xziqi.cn/gtxoimqcxa.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtejsdqlmd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangshuangyany.cn/gtlysjssxk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhoulong.xyz/gtreytjzke.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gtbzytfufq.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtuopyetrx.html

Py:   self.name = "x"
来源：http://hz.wangdashe.top/gtdvuusoug.html

PHP:  public string $name = "x";
来源：http://hz.ydjk.org.cn/gtldtqtvax.html

JS:   this.name = "x";
来源：http://hz.shuidangran.top/gtznadjnaz.html

TS:   name: string = "x";
来源：http://hz.xingfuxueyuan.xyz/gtxboilcsa.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtngmftbro.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.mhx1999.top/gtaxjqxmlg.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtwxcihptj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jianghu66.top/gtyfksgwoi.html

[G04] 定义方法
来源：http://hz.aizwys.cn/gtjcyrdqyy.html

Py:   def greet(self): return self.name
来源：http://hz.smart0.xyz/gtwhornwvd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtfuhlqcih.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtfzcvoxpm.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtfdmwdpsm.html

Java: String greet() { return name; }
来源：http://hz.guowangkeji.top/gtnnfnvuoc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gthhwwwfbq.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtuxvsmhqx.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gtcddneqer.html

[G05] 继承
来源：http://hz.sweek.top/gtlzdcizan.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtmvcttqki.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gttkhndmfv.html

JS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtxazpsxcr.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtkwmwlbsi.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtnwnwnhwg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tianlin.xyz/gtukvbolew.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtecnjfjhb.html

C#:   class Admin : User {}
来源：http://hz.andypj.xyz/gthzxzhayg.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtvdhzwelt.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtyswiivua.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtfjwgcihh.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gttwtdntmh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtggijtvef.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtfvxunhca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gthexciyhk.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtozwrkjmm.html

C#:   public override string Greet() => "admin";
来源：http://hz.yonumen.top/gtcecbfabd.html

[G07] 调用父类方法
来源：http://hz.cheryme.top/gtmgqvkvkj.html

Py:   super().greet()
来源：http://hz.gaohongyu789.top/gtuxffghkv.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gthocwhnun.html

JS:   super.greet();
来源：http://hz.aizwys.cn/gtrsrjdwzs.html

TS:   super.greet();
来源：http://hz.fengsongda.top/gttlhywejo.html

Java: super.greet();
来源：http://hz.zhoulong.xyz/gthnzmtznu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtazwkmuum.html

Ruby: super
来源：http://hz.pengpengdd.cyou/gtnitgkrmz.html

C#:   base.Greet();
来源：http://hz.hfpthk.cn/gtdunmfgdn.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtpliomkiv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxuanxn.top/gtsskjtbyn.html

PHP:  public static function f() {}
来源：http://hz.gzhubu.top/gtsdlhxxal.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gtajsehzzt.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtrktnqxau.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtgkozopne.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtvxynwebs.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gtaztytstl.html

C#:   public static void F() {}
来源：http://hz.jqgufenzy.top/gtnvvskjdp.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gtgslevvfi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yongpay.top/gtlrqxcrrm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtenysamxq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cdnleiting.top/gtbfuuxhen.html

TS:   interface Shape { area(): number; }
来源：http://hz.haohaochexian.top/gtxjtfbayw.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258888.top/gthoykbxqs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gtoafnfviw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.svipenyu.cn/gtzicpipvh.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gtyuzwgmke.html

[G10] 访问控制
来源：http://hz.ybcxt.top/gtufgcpgfc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtkkstdexe.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtvglsuxqt.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtyaaeokvg.html

TS:   public / protected / private
来源：http://hz.dashuyun.cn/gtxycmcsdu.html

Java: public / protected / private / 默认包级
来源：http://hz.nwbrower.top/gtsjyhfweq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hammf.cn/gtmynphmqi.html

Ruby: public / protected / private
来源：http://hz.yuanzhike.top/gtlywxpkda.html

C#:   public / protected / private / internal
来源：http://hz.52xcode.cn/gtvzvqueli.html

[G11] getter / setter
来源：http://hz.ppjwa.cn/gtzszfbloi.html

Py:   @property 与 @x.setter
来源：http://hz.daria6918.cn/gtgcdmmdbr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtnfyllpne.html

JS:   get name() { return this._name; }
来源：http://hz.ehwqpu.com/gtchhzrmdl.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtzdrqkybs.html

Java: public String getName() { return name; }
来源：http://hz.yongpay.top/gtxtjksomc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydzc1.top/gtvyjsanxp.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtijesmuei.html

C#:   public string Name { get; set; }
来源：http://hz.ydjk.org.cn/gtkcopcieb.html

[G12] 对象转字符串
来源：http://hz.gzhubu.top/gtmskfxhvi.html

Py:   def __str__(self): return self.name
来源：http://hz.hnqzz.top/gtrjsqwifn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtsxiiyrzs.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtlorcbkga.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuxming.cn/gtjbgtrkev.html

Java: @Override public String toString() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtcfuniweh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xylfe.cn/gtdskabiql.html

Ruby: def to_s; @name; end
来源：http://hz.jianghu66.top/gtkijuqvbd.html

C#:   public override string ToString() => Name;
来源：http://hz.zhijiandao.cn/gtkduoqvkt.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtsyzptdea.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gtmgtohspe.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtmnyzkhea.html

JS:   u instanceof User
来源：http://hz.ivvv.top/gtjhezpoym.html

TS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtibgivwnj.html

Java: u instanceof User
来源：http://hz.chenlongwang.top/gthvwflvey.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinyuanbaomall.cn/gtlsqxuilb.html

Ruby: u.is_a?(User)
来源：http://hz.haohaochexian.top/gtpvuvmcjc.html

C#:   u is User
来源：http://hz.sxryk.cn/gtanomdkot.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtxiydhywd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuetiantiany.cn/gtuepzwozd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gtaoddcbbk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.birdmap.top/gtkegrdscz.html

TS:   type User = { name: string; age: number };
来源：http://hz.cqqwz.cn/gtienpcjov.html

Java: record User(String name, int age) {}
来源：http://hz.xziqi.cn/gteamsmgys.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gteomakuyg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gtqdlsqsob.html


<!-- 参考信息 -->