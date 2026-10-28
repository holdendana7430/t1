代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gthyebaxlu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtqlcltlpa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gtuvlrpbrg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guowangkeji.top/gtactkygqn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.redwolf501.top/gtijlzpacf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtqiwylvlz.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gttrjrdcvj.html

Py:   f"{1234567:,}"
来源：http://hz.jyoumei.cn/gtjbvfwvqa.html

PHP:  number_format(1234567);
来源：http://hz.ppjwa.cn/gtdglykrst.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtnliopkmz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gttpiqkjze.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangkeji.top/gtvnxvvzvi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtrykhmznw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tian-w.cn/gteahopnix.html

C#:   1234567.ToString("N0")
来源：http://hz.iojbl.cn/gthrjadvqu.html

[E17] 首字母大写
来源：http://hz.hfpthk.cn/gtsmjfxulw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhengqikj.top/gtbwwoktvo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtabfzzeiv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtqotuzldu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gttaygjynn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtpxzmvsac.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgufenzy.top/gthtwytpal.html

Ruby: s.capitalize
来源：http://hz.jqgfzy.top/gtvhxjchnh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtejckrkfd.html

[E18] 模板占位符替换
来源：http://hz.hongshengwenyu.top/gtyrwljrht.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtkmznrvpy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gtaieljwjy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtukmnqseg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtcsbcbbyd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtujeqmhhj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtxrxmuryk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yueranfly.top/gtqcdsapte.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gzhubu.top/gtowpypqrh.html

[E19] 多行文本按行拆分
来源：http://hz.cheryme.top/gtiembourz.html

Py:   s.splitlines()
来源：http://hz.tianlin.xyz/gtuvwvrept.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydzc1.top/gtcbvwnrxc.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtewgojwul.html

TS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtnjxsjtuz.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangtech.top/gtehtjlckr.html

Go:   strings.Split(s, "\n")
来源：http://hz.c1oappe.top/gtqwecrrpx.html

Ruby: s.lines
来源：http://hz.redwolf501.top/gtjcbnuymx.html

C#:   s.Split('\n')
来源：http://hz.gotoacloud.top/gtsmjrkrdc.html

[E20] 判断字符串是否为空
来源：http://hz.shuidangran.top/gtvofasblv.html

Py:   if not s:
来源：http://hz.ivvv.top/gtdcyiclzk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtgloqsvke.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtawztmylx.html

TS:   if (s === "") {}
来源：http://hz.gotoacloud.top/gtdbkxqbkp.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtoospkwah.html

Go:   if s == "" {}
来源：http://hz.zhixingplan.top/gtkgudlvxo.html

Ruby: if s.empty?
来源：http://hz.hammf.cn/gtgsynpvra.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtsxaiwbtq.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtschgekwf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangkeji.top/gtqxcevnzm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtlkgcdlec.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtylkinegj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtnzbuyevi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtsknrxkrm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gttgzluhqv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtevznnbeq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtyefxifqr.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtowgostxq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangdashe.top/gtslgmdotk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhixingplan.top/gtotzihdhj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtjapcifok.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtledkgpxc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shzxlz.cn/gtlpwnwifi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cashguo.top/gtghqrygjn.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtpokutann.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daria6918.cn/gtlbpcmzuf.html

================================================================================
来源：http://hz.snrcjt.cn/gtesjhalkt.html

F. 文件与目录
来源：http://hz.jlsjyb.cn/gtyvflxtfm.html

================================================================================
来源：http://hz.ydjk.org.cn/gthmqiklli.html

[F01] 读取整个文件
来源：http://hz.kuanghao11.cn/gtaletsjvc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtwokeueee.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hammf.cn/gtgpobrxug.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtdqliqpfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtsqelkrsg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtgjvsmxhp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cdnleiting.top/gtdbbjbwwo.html

Ruby: File.read("a.txt")
来源：http://hz.9152youxi.cn/gtllsotqza.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtocaxymkp.html

[F02] 逐行读取文件
来源：http://hz.xuanzx.com/gtcryvjdox.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtyixieteg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yangfankeji.com/gtvrqeihpn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtfywlduxh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gtgipzbzcf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtzevvhgjg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtbahbtjvq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hammf.cn/gtrbxmwpzh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtjdhlzltn.html

[F03] 写入文件（覆盖）
来源：http://hz.cdnleiting.top/gtizkqbozk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtrfabjwwo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gttabnmpfm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtyyectkjk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtlyeitivh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhixingplan.top/gtykcvitzv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yanxiufei.cn/gthnfuogap.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtgmxdnuet.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gthmkvhqwl.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtpdahfife.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtbycoefxu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj202588.top/gtvburmhpu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtcmxtejvp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtityuehug.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dianchejie.cn/gtxtikcrka.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtspzfhvpb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtlsfqfomq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtstpujwdk.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtrrotqgka.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgfzy.top/gttfuvnelb.html

PHP:  file_exists("a.txt");
来源：http://hz.cqqwz.cn/gttrsvojxp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtreksahsl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtampgryny.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtjbuwozxl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtwxbnwbwv.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj202588.top/gtfttldlre.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtzqhlyyis.html

[F06] 删除文件
来源：http://hz.yj202588.top/gtnmlkirga.html

Py:   os.remove("a.txt")
来源：http://hz.zycfv.cn/gthgmrxmop.html

PHP:  unlink("a.txt");
来源：http://hz.mhx1999.top/gtlgtfbnts.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gthyubskuq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtjrsrhbao.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtonemmtmi.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gtzfopslza.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtdozqustw.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtzmtrcpqw.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtqsnrwune.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtmaqxmhvo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangshuangyany.cn/gtugjnmmeo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtlykmmnjh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtohwhibiw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnxiangtu.top/gtnilwclqn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtdmnufcsf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydjk.org.cn/gtpandukrb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtboojtlka.html

[F08] 遍历目录
来源：http://hz.yj20258888.top/gtonehepjs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtzifnwkic.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtmemjmvbn.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtnikxbcvx.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtpfbezhcd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtetfsaunn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gtyvinmpzp.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtoyqbplvw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jyoumei.cn/gtcqcdggdx.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gtayzsacai.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtolwcrpcp.html

PHP:  filesize("a.txt");
来源：http://hz.yongpay.top/gtzxjyyarn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtktgidyls.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtyspymjxl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gthgmdjkkb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtqakgmcyq.html

Ruby: File.size("a.txt")
来源：http://hz.jianghu66.top/gtzuslvznx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhixingplan.top/gtuavafrhp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gtlcofbwho.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtpybryyfg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtbugcbwib.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtnnshbhlx.html

TS:   path.extname("a.txt")
来源：http://hz.xuanzx.com/gtusrcxylg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gotoacloud.top/gtluthlxiz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtuvixqwmr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtopucbxia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gtikjesduo.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtnbmprbxy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtzrlaejzj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtinpnxjhb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtclyaweql.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gttgpktkue.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.kuanghao11.cn/gtywxrzkiy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tanke756.top/gtyuerlbgo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtkwgslqqx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtpeejiutr.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtdrlbrexp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tianlin.xyz/gtezodcuzk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtrqowxocn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shangyingyoupin.top/gtmgamhthf.html

TS:   // 同上
来源：http://hz.aizwys.cn/gtrrkffpag.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtyfeffnro.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtimmekgmm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtxarlmxii.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhiwuduotai.top/gtlgypthnc.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkvbbxjfu.html

G. 面向对象
来源：http://hz.shzxlz.cn/gtltwfvcua.html

================================================================================
来源：http://hz.jyoumei.cn/gtyehnpkym.html

[G01] 定义类
来源：http://hz.zhongyouzk.top/gtemzazpdd.html

Py:   class User: pass
来源：http://hz.nanxuanxn.top/gtcwqaksgb.html

PHP:  class User {}
来源：http://hz.shanyushiyangtech.top/gtnacjyodn.html

JS:   class User {}
来源：http://hz.svipenyu.cn/gtdepdamoe.html

TS:   class User { name: string = ""; }
来源：http://hz.zhengqikj.top/gtlweqjifj.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtyiwpserd.html

Go:   type User struct { Name string }
来源：http://hz.zdqjudy.top/gtrpwfhaew.html

Ruby: class User; end
来源：http://hz.fzhhl.top/gthsptlswy.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gtwekjdnuu.html

[G02] 构造函数
来源：http://hz.fengsongda.top/gtwqdlyngs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtryzxakfn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hammf.cn/gtloarjyko.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.c1oappe.top/gtfxlwusdv.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtwwidqylg.html

Java: User(String name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtketfrgug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtufrhcavz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nwbrower.top/gtaccrflfq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.bjfxy.top/gtyuupqhzh.html

[G03] 实例属性
来源：http://hz.wangshuangyany.cn/gtwhktgbgw.html

Py:   self.name = "x"
来源：http://hz.chenlongwang.top/gtlupkkhlk.html

PHP:  public string $name = "x";
来源：http://hz.hnxiangtu.top/gtkkxytjdt.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtwomwfisf.html

TS:   name: string = "x";
来源：http://hz.jinqigfzy.top/gterrbzsji.html

Java: private String name;
来源：http://hz.xziqi.cn/gtyzspjqaq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dianchejie.cn/gthzhofdng.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gthlnaghad.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtdicssftc.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtctpnnitd.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtdlllaths.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtqwxcoeft.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtnfduqnsg.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtjidpqtsy.html

Java: String greet() { return name; }
来源：http://hz.zhongyouzk.top/gtjiihlwhc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.daxiang520.top/gtexleyufw.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtsflsbtcc.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtdvsmtekh.html

[G05] 继承
来源：http://hz.xinyue.icu/gtdzizzacj.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gthbrvxdyw.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtultfjmrw.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtlwfltdgk.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtkpmmmomh.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtqapgyirm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gtvjvhueht.html

Ruby: class Admin < User; end
来源：http://hz.jqgfzy.top/gtouhjldav.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtjudzwbco.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtrwphajbj.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtzmyqzhup.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtbvhoesaf.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtmsdqzfwl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtsbnqmlyn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtnxrnbprm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtnnzwxumx.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtcnwdonaj.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtmmmgtfmg.html

[G07] 调用父类方法
来源：http://hz.hnxiangtu.top/gtmgjweslz.html

Py:   super().greet()
来源：http://hz.yj20258.top/gtpvdojphg.html

PHP:  parent::greet();
来源：http://hz.xinyue.icu/gtmsvhfqox.html

JS:   super.greet();
来源：http://hz.316326.xyz/gtwlutnfin.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtrqedgobj.html

Java: super.greet();
来源：http://hz.aizwys.cn/gtojjrjoai.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shuidangran.top/gtirycpjqt.html

Ruby: super
来源：http://hz.chenlongwang.top/gtpnxbytwj.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtsvdpictq.html

[G08] 静态方法与属性
来源：http://hz.redwolf501.top/gthjndaoyo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gteqhvjqtx.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gtvggydpye.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtnzrkdlar.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gthykixctj.html

Java: static void f() {}
来源：http://hz.xziqi.cn/gtdryeqsfz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtripipdif.html

Ruby: def self.f; end
来源：http://hz.jinghuilouyu.cn/gtretvukob.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gtnnqnmsex.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtsygzxbcl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtprwajiba.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtkwvtvfhj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtbbuiqrir.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtmejfeesv.html

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gtcupsrfdy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gttwtevcrv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cheryme.top/gtrewkbogb.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtzpdisorw.html

[G10] 访问控制
来源：http://hz.fzhhl.top/gtbmpehybd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtglthsrvx.html

PHP:  public / protected / private
来源：http://hz.quarkkingdee.top/gtjmjhvdlh.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gthjxtbcps.html

TS:   public / protected / private
来源：http://hz.316326.xyz/gtbwacjpqh.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtdmuznkkz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.snrcjt.cn/gtviochjmx.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtxvdpldcp.html

C#:   public / protected / private / internal
来源：http://hz.nwbrower.top/gtsjsxvlpe.html

[G11] getter / setter
来源：http://hz.jinqigfzy.top/gtrzwrslhl.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtreztiknz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtrcwgmjkg.html

JS:   get name() { return this._name; }
来源：http://hz.vqdsnc.cn/gtqozvicxf.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtvgayxyjd.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtvwkmburg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtgyybctij.html

Ruby: attr_accessor :name
来源：http://hz.vqdsnc.cn/gtrkwpdsxv.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtblbelmnx.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtvsvufaby.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtiizeegzx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gttxzfhgfe.html

JS:   toString() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtccixbvnv.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtxfwrkycp.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtrhzsotue.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtyltpedrx.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtwfmzsdlg.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtjfhfrukm.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gtguukngvb.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gtliuczglx.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtdddwflyo.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gtezrxwpal.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtpazmgfls.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtqmwtdiny.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtsddixtjv.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gtmkfahmms.html

C#:   u is User
来源：http://hz.316326.xyz/gtsluquvhi.html


<!-- 参考信息 -->