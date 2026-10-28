代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sxryk.cn/gthpbftmiu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangtech.top/gtvxhrcmmz.html

[E16] 数字千分位
来源：http://hz.cqqwz.cn/gtwsiafmoh.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtssgiyoeb.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtzypogfub.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtnksbbkbd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtrgorvicq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenjidiqi.icu/gtuyhxuqmz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sweek.top/gttwhyvrbi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gogol.net.cn/gtejqyhtru.html

C#:   1234567.ToString("N0")
来源：http://hz.yvedp.cn/gtyxuzukee.html

[E17] 首字母大写
来源：http://hz.zhixingplan.top/gtznidswpz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtagrhtnbm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgufenzy.top/gtnxmffeoq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtaxsitojz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtyizyvohr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tian-w.cn/gtksrkvnoc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gttmskqmbb.html

Ruby: s.capitalize
来源：http://hz.yangfankeji.com/gtscsdvgxp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shzxlz.cn/gtwipmaotl.html

[E18] 模板占位符替换
来源：http://hz.dashuyun.cn/gteyerccpo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinqigfzy.top/gtsyhqavcz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gttyiiqmho.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtuwvfjexj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gthzakoygr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tanke756.top/gtkjphcyrc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.andypj.xyz/gtokywblll.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daxiang520.top/gtdopqjynh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxuanxn.top/gtovmusxfj.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtcwwbbotq.html

Py:   s.splitlines()
来源：http://hz.zhengqikj.top/gtmetubfus.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gtpfmxectm.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gthgxlxjey.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangtech.top/gtcunktsah.html

Java: s.lines().toList()
来源：http://hz.yueranfly.top/gtptpvyvyo.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtdytmswxr.html

Ruby: s.lines
来源：http://hz.c1oappe.top/gtyvqqicjr.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtfyyyhvwr.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtdpviojed.html

Py:   if not s:
来源：http://hz.andypj.xyz/gtgtlbmbod.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zycfv.cn/gtbxivofov.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtjxxeolvz.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtqghihzov.html

Java: if (s.isEmpty()) {}
来源：http://hz.svipenyu.cn/gthggjqvld.html

Go:   if s == "" {}
来源：http://hz.smart0.xyz/gtenbkerjq.html

Ruby: if s.empty?
来源：http://hz.gaohongyu789.top/gtdaftztln.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtjzrddemh.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gteawsgnyp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zdqjudy.top/gtseonzbou.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtcptvvmgj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtqkdfzqcx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtiwfhvwwq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtmatmiakr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgufenzy.top/gtfbxxpijw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zycfv.cn/gtjwhsects.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtkcodioxv.html

[E22] 字节长度与字符长度
来源：http://hz.pycfn.com/gtowcysrtx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.feifeiyinyue.top/gtdtyfcsey.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtzhexvllj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gthbespyru.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cdnleiting.top/gtvgciyxtx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtzuabhuaf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinyuanbaomall.cn/gtxrelopdg.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtuxnxphla.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gttgpjwpxk.html

================================================================================
来源：http://hz.yj202588.top/gtvlhjqfje.html

F. 文件与目录
来源：http://hz.yuanzhike.top/gtuddssgpj.html

================================================================================
来源：http://hz.ydzc1.top/gtqwrrazfg.html

[F01] 读取整个文件
来源：http://hz.fengsongda.top/gtijlgarou.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtpgknbwru.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gtjswdcdan.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gtkeakjnnh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.kuanghao11.cn/gtecyswsvy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtfykgjosj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.havefunace.top/gtmfzpoxgq.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtetsmlfhn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zdqjudy.top/gtianbbfsh.html

[F02] 逐行读取文件
来源：http://hz.hnxiangtu.top/gtkfqvliuo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sysykeji.top/gtpsqgmdus.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gogol.net.cn/gttlzvaryr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtfitagawm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtiigrquac.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtevfktraq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigufen.top/gtjvrpyqrq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtkmmyevly.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangdashe.top/gtspeaxgfd.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtjuqflxgl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangdashe.top/gtnmsgwhis.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtbcdzypyd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtvcxeffpv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daxiang520.top/gtoopiqmrd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhoulong.xyz/gtdzdrjnte.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gthtrhqneb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtiotnsewt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtpuaetplo.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gttgpclufu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shzxlz.cn/gtdmzsjwnw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ivvv.top/gtfctngasb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtlqpvixuv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtvksdvrhd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aizwys.cn/gtescwivgy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gogol.net.cn/gtjfzhfskz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenjidiqi.icu/gtmpwgfnpn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhongyouzk.top/gtfbbeffba.html

[F05] 判断文件或目录是否存在
来源：http://hz.havefunace.top/gtgaalkgiu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.iojbl.cn/gtijjmiily.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgfzy.top/gtrbvlhytp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtkmyoppbu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtfliigbjb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtglnljisq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sweek.top/gthcghaldg.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtrlaxtlqz.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtiwagvsdx.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gtrebpfpqy.html

Py:   os.remove("a.txt")
来源：http://hz.gzhubu.top/gturwajrff.html

PHP:  unlink("a.txt");
来源：http://hz.guowangkeji.top/gtxayctnuv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtllgykzpn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtdlqbrccz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtpfkdwhjq.html

Go:   os.Remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtfwwdrrhc.html

Ruby: File.delete("a.txt")
来源：http://hz.jianghu66.top/gtmjzdsvic.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gtfgxfijmp.html

[F07] 创建目录（含多级）
来源：http://hz.ppjwa.cn/gtdppcdmci.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cdnleiting.top/gtterldhgf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guowangkeji.top/gtghialjpj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtqduiwksj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtdfcmgfxd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.quarkkingdee.top/gtosdpvnbf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.0kj1m.cn/gtgimzseax.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yonumen.top/gtjkwpfubx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtarvyiuso.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gtvbdmmzoq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.svipenyu.cn/gthvmxnouz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gotoacloud.top/gtvurpcfjx.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtbokfiaod.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtissazsxj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gttejdqjkp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gttprmvduo.html

Ruby: Dir.children("dir")
来源：http://hz.cdnleiting.top/gtaqvckyqk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnqzz.top/gtvlyayyrd.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtmxnvuoqz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gtdgubvmfc.html

PHP:  filesize("a.txt");
来源：http://hz.dashuyun.cn/gtsbyaworo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtfmssfjax.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtirqcpxbm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtunfkmprc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gtbaqrnefv.html

Ruby: File.size("a.txt")
来源：http://hz.kuanghao11.cn/gtacphrdkp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gtwvqnykhe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtjqkduwiw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtrpcdaxyt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daxiang520.top/gtevtgldmm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtxqeqnxrc.html

TS:   path.extname("a.txt")
来源：http://hz.bjfxy.top/gthybortbn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtwkinrqxc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guowangkeji.top/gtoxwculxp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtkeqnymfw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.redwolf501.top/gtjmixrchc.html

[F11] 复制与移动文件
来源：http://hz.pycfn.com/gtxcmavygl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gteaazyowe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.meibo888.top/gtlxjbwjue.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gthzkpubld.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtkxyyymix.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhoulong.xyz/gttqiexubu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtdshhcson.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtgbichuks.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtjmcslhod.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtfovwvcwo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtztgpgwiv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gtjozzwhzs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtisekvyug.html

TS:   // 同上
来源：http://hz.yvedp.cn/gttfbhfkeq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtizpyfocv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xylfe.cn/gtmfqnbzab.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtinozwkim.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hysaishi.cn/gtzttdvgxb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqavjdurj.html

G. 面向对象
来源：http://hz.gogol.net.cn/gtdzkzrjpc.html

================================================================================
来源：http://hz.zycfv.cn/gtenxompga.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gthjoyfoik.html

Py:   class User: pass
来源：http://hz.hysaishi.cn/gtkghasisx.html

PHP:  class User {}
来源：http://hz.zhongyouzk.top/gtjovznasc.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtjhionvad.html

TS:   class User { name: string = ""; }
来源：http://hz.iojbl.cn/gtwqasnlcj.html

Java: class User {}
来源：http://hz.hnxiangtu.top/gtjzeiegmt.html

Go:   type User struct { Name string }
来源：http://hz.kuanghao11.cn/gtmlellysm.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtqbvwoenb.html

C#:   class User {}
来源：http://hz.ppjwa.cn/gtzblrimdl.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtnnvvvlby.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.meibo888.top/gtlxkswtxn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhengqikj.top/gtmlqqxldz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtkkwlqupa.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtqpklocvv.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtvlbkndui.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtikvagoid.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtwrujlqed.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gtxardkwec.html

[G03] 实例属性
来源：http://hz.jinghuilouyu.cn/gtusnmgbzh.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtftozqyxi.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtdltjrtcq.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtmaqfepnw.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtnyepzuqj.html

Java: private String name;
来源：http://hz.redwolf501.top/gtpraxqzsm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtdtsigtdj.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtvxjpiefk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hongshengwenyu.top/gtudgwmlbb.html

[G04] 定义方法
来源：http://hz.ehwqpu.com/gtmxqzvtbs.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtvwolmrhi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gthfdznhho.html

JS:   greet() { return this.name; }
来源：http://hz.guowangkeji.top/gtkcerbooa.html

TS:   greet(): string { return this.name; }
来源：http://hz.guannengcc.top/gtuqxnrwek.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtndhhjjqr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cheryme.top/gtdcechcmb.html

Ruby: def greet; @name; end
来源：http://hz.sxryk.cn/gtskhsmnwv.html

C#:   public string Greet() => Name;
来源：http://hz.hysaishi.cn/gtyorcquzh.html

[G05] 继承
来源：http://hz.jianghu66.top/gtddptbqvk.html

Py:   class Admin(User): pass
来源：http://hz.zycfv.cn/gtwewatgnd.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gtnkacigjd.html

JS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtpcnhuskt.html

TS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtlujofusr.html

Java: class Admin extends User {}
来源：http://hz.iojbl.cn/gtrsrmhcnk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shuidangran.top/gtnczqcihf.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtmtlotaxk.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtpzqdxldg.html

[G06] 重写方法
来源：http://hz.ybcxt.top/gtttzkdysl.html

Py:   def greet(self): return "admin"
来源：http://hz.ydzc1.top/gtmlfdnuhi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtdmqbjblf.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtrxqpmkyh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtcoqudsht.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtebikppvn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dashuyun.cn/gtqpkuyzeb.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gtbymkiren.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtyltqhxqo.html

[G07] 调用父类方法
来源：http://hz.yj20258888.top/gtnjpnoafz.html

Py:   super().greet()
来源：http://hz.sysykeji.top/gtshktmyza.html

PHP:  parent::greet();
来源：http://hz.havefunace.top/gtuuvypfsk.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtvfdsmfdp.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtvkliqyos.html

Java: super.greet();
来源：http://hz.daria6918.cn/gtbjcisrxe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtpfyglmcq.html

Ruby: super
来源：http://hz.zhoulong.xyz/gtlwqtojwg.html

C#:   base.Greet();
来源：http://hz.cheryme.top/gtcgzqtapn.html

[G08] 静态方法与属性
来源：http://hz.yanxiufei.cn/gtksekirvv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtdcdzymcc.html

PHP:  public static function f() {}
来源：http://hz.aizwys.cn/gthcrrnxov.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtciitzyyq.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtyzagwmnq.html

Java: static void f() {}
来源：http://hz.xingfuxueyuan.xyz/gtqepdqxvs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgufenzy.top/gtyfizocif.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtcjexpjhn.html

C#:   public static void F() {}
来源：http://hz.hnxiangtu.top/gtxkrfabfa.html

[G09] 接口 / 抽象类
来源：http://hz.jiagoushi.top/gtkqenfrdg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnqzz.top/gtghqsettj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gthddxwvfx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtchmltmvi.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtfcjvrmes.html

Java: interface Shape { double area(); }
来源：http://hz.yangfankeji.com/gtngjzvmja.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yueranfly.top/gtbmxclvup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtrpnqhqzl.html

C#:   interface IShape { double Area(); }
来源：http://hz.sxryk.cn/gtqehslndv.html

[G10] 访问控制
来源：http://hz.ydzc1.top/gtwnzrnprz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xinyue.icu/gtqprnvrbe.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gthbetifzk.html

JS:   #private 字段；其余公开
来源：http://hz.svipenyu.cn/gtmyiumwuc.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtbvlzsqah.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtjbxahbzl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gtknsxwsud.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtuvpbfibc.html

C#:   public / protected / private / internal
来源：http://hz.pycfn.com/gtcbbojagz.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtypjqkdfp.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtejqhddzu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtxwhxxnec.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtdyasckvo.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gtpxidrsox.html

Java: public String getName() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtluabfiod.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtiamhgwsv.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gthuemtrbd.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gttwegqsfs.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gttwesrvye.html

Py:   def __str__(self): return self.name
来源：http://hz.kuanghao11.cn/gttegdoton.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtltskdqup.html

JS:   toString() { return this.name; }
来源：http://hz.yueranfly.top/gtsuqjtnmq.html

TS:   toString(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gthpzrbioo.html

Java: @Override public String toString() { return name; }
来源：http://hz.sufxvd.cn/gtbyyamxqi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtvddiqmzr.html

Ruby: def to_s; @name; end
来源：http://hz.ywan-chungtsiang.top/gtbpypmreg.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtsvigxgag.html

[G13] 判断对象类型
来源：http://hz.dianchejie.cn/gtshljhvnq.html

Py:   isinstance(u, User)
来源：http://hz.ppjwa.cn/gtqlchzjxe.html

PHP:  $u instanceof User
来源：http://hz.shuidangran.top/gthgbynjxi.html

JS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtxjangtsu.html

TS:   u instanceof User
来源：http://hz.gzhubu.top/gtkaodsctt.html

Java: u instanceof User
来源：http://hz.316326.xyz/gtpwbkwjmt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yongpay.top/gtzgdtoorz.html

Ruby: u.is_a?(User)
来源：http://hz.jinghuilouyu.cn/gtxmosygpg.html

C#:   u is User
来源：http://hz.xinyue.icu/gtrlyymmys.html

[G14] 数据类 / record
来源：http://hz.ydzc1.top/gtwvtobsri.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenzaomai.com/gtztnfiknm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gtcgnqkkce.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gtjdullpym.html


<!-- 参考信息 -->