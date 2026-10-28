代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ybcxt.top/gtzurdronp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gthwcqgcsj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gtlazoeayl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.meibo888.top/gtwziwnzsr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtgdhfbair.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhoulong.xyz/gtxcjjbfvo.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtbjrbkdxq.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258.top/gtgoytsvsg.html

PHP:  number_format(1234567);
来源：http://hz.ppjwa.cn/gtttwhwxkc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtaxnqfpyi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtxssvnvkq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ehwqpu.com/gtkcvsifzg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.316326.xyz/gthbjmbuwq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shuidangran.top/gtmxpeftgx.html

C#:   1234567.ToString("N0")
来源：http://hz.yongpay.top/gtexzutocz.html

[E17] 首字母大写
来源：http://hz.yonumen.top/gtmfvlftvm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhiwuduotai.top/gtqjhddfjw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tianlin.xyz/gtvvilaudu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtizuiijvu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtuefmarwa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtnwisilqt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gtfeyeshht.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gtkptkycdw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhengqikj.top/gtfzscoddn.html

[E18] 模板占位符替换
来源：http://hz.yuanzhike.top/gtvotctywu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtqgbmubyw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tanke756.top/gtkscsztnq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtpjdosvyi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtmzhocykz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xylfe.cn/gtmxizecis.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgufenzy.top/gtrxqbibdi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnqzz.top/gtkptdqnng.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jiagoushi.top/gtlvrzaqum.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtbjyuaqjo.html

Py:   s.splitlines()
来源：http://hz.ywan-chungtsiang.top/gtbhqmscpv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgfzy.top/gthxgarwxg.html

JS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gthjpolcvj.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtjiepxrwk.html

Java: s.lines().toList()
来源：http://hz.sysykeji.top/gtkxjbuyjp.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtfvxzlzkm.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtxgfnownj.html

C#:   s.Split('\n')
来源：http://hz.fengsongda.top/gtspvdmoyv.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gtmiifxzao.html

Py:   if not s:
来源：http://hz.gzhubu.top/gtofklexxv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gtkbzgzlbs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cashguo.top/gtckpvoedt.html

TS:   if (s === "") {}
来源：http://hz.tianlin.xyz/gtipvgsjiz.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtwinrvkub.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gtjzzxbzoc.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtdfbfigju.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtgvzciuen.html

[E21] 超长截断加省略号
来源：http://hz.wangdashe.top/gtfzxpcibp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtnszwoyyi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guannengcc.top/gtrdoxhukr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtqhbkcexp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gthfferzdx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtdebfwzxk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtubonmess.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgfzy.top/gtwwevazqh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dashuyun.cn/gtscylkkzo.html

[E22] 字节长度与字符长度
来源：http://hz.havefunace.top/gtxjygrgdd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.havefunace.top/gtwsxapytf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtjhesxtxo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtqmupbzru.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtvvrkvlaz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtedgirnrb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtserwrigc.html

Ruby: s.bytesize;  s.length
来源：http://hz.iojbl.cn/gtvamqgnhx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ydjk.org.cn/gtyefblwqk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjevxkrdp.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtwpybsdfy.html

================================================================================
来源：http://hz.ehwqpu.com/gtdrgkiuyp.html

[F01] 读取整个文件
来源：http://hz.nanxuanxn.top/gtbyxmpotz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gaohongyu789.top/gtqianrgxt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.daria6918.cn/gtjlnumxyk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shzxlz.cn/gtetvvtecr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tianlin.xyz/gtxeordpna.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gteogifjkz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtfczpxcyu.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangtech.top/gtuqloruld.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zdqjudy.top/gtslquaumr.html

[F02] 逐行读取文件
来源：http://hz.hnqzz.top/gtkzrtcaag.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dashuyun.cn/gtjnstrdrn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtrdzaysvr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtrcidpoow.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtbkrhmjsy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gthhcfdyvu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hfpthk.cn/gthmxjrodm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenjidiqi.icu/gtlebihxgf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gzhubu.top/gtwyfokjxi.html

[F03] 写入文件（覆盖）
来源：http://hz.shzxlz.cn/gtgxijazmz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.smart0.xyz/gtqpezvbbc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtpzswedti.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtwhmvbrnr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtdyuyqimn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gtqjcdlvnb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sufxvd.cn/gtsmgaecxp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jiagoushi.top/gttgmgteyj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtquvftwnn.html

[F04] 追加写入文件
来源：http://hz.ywan-chungtsiang.top/gtyzqpnoxo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhaomingkeji.xyz/gtwbrvcvln.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtxniqxwcv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtlzvohvyq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtkjoqexoa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gtlbflbzvu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtwucjflrf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtpfxbqbhn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gtvykcxbda.html

[F05] 判断文件或目录是否存在
来源：http://hz.shuidangran.top/gthiypxrsj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtjmliuott.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtkuwsmqfj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtepidemdi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtqfjqxsqf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtpvftqvhb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cucudq.cn/gtjzqxrhen.html

Ruby: File.exist?("a.txt")
来源：http://hz.bjfxy.top/gtnxqenftq.html

C#:   File.Exists("a.txt")
来源：http://hz.zhongyouzk.top/gtjpdxcocv.html

[F06] 删除文件
来源：http://hz.shangyingyoupin.top/gtpctjclwh.html

Py:   os.remove("a.txt")
来源：http://hz.tianlin.xyz/gtttdszmix.html

PHP:  unlink("a.txt");
来源：http://hz.yanxiufei.cn/gtfdejielj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtnrayuxob.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtpxkcezkr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gttgyaoudl.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtskunfvwx.html

Ruby: File.delete("a.txt")
来源：http://hz.bjfxy.top/gtyyfzqwbv.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtkormopia.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtasrmedil.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtidzjhfgw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtwgvolwuf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtsotxyycl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtqnariord.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtjifuhwum.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtndxzaysu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gtwauamllr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtaxprcynm.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gtgytvftnz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtjhegrtct.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fengsongda.top/gtintkfcfy.html

JS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtkecpaueq.html

TS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtdugmnoqu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtlpvihzvs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinyuanbaomall.cn/gtkhecflmx.html

Ruby: Dir.children("dir")
来源：http://hz.guowangkeji.top/gtrqmxcmjj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yvedp.cn/gtmzkwfzmu.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtoshtizvb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtwpkaqoyp.html

PHP:  filesize("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtqhgsldec.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtsctrrmgx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gteiiltnsv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtfgpagghy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gzhubu.top/gtyxvrstmx.html

Ruby: File.size("a.txt")
来源：http://hz.hammf.cn/gtrhsjeunu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtcrpujamh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtnmhlxpqw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtlcbrwxcp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zdqjudy.top/gtlwwoxrtw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtbqsnpdes.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gtqfedeosn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtiqzwuiiv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtaqskzbif.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtfdzmjevm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fengsongda.top/gtzpjxfwlx.html

[F11] 复制与移动文件
来源：http://hz.feifeiyinyue.top/gtnmtpygol.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtnvnorgzg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinyuanbaomall.cn/gtjybpsavr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtbdcemqlf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtyiqvtqqt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtiblfefsv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daria6918.cn/gtawregtha.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtxcvspwut.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gthbtucmjs.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtfbgzpmpt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtpcycyono.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aibaodan.cn/gtgoiyaahp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ivvv.top/gtiomrsydd.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtmmgvoyrq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shangyingyoupin.top/gthwkqedxn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtpkgqsull.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtcfdejflf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtghddflhw.html

================================================================================
来源：http://hz.yongpay.top/gtgxvhktzw.html

G. 面向对象
来源：http://hz.ehwqpu.com/gtmexcgzen.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjeysuhac.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtanjdxtqh.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtxlextkfo.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtwrfvsimg.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtfxeskjqv.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gtuzcrakla.html

Java: class User {}
来源：http://hz.gotoacloud.top/gtbgjvthch.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtjipmwgbf.html

Ruby: class User; end
来源：http://hz.cashguo.top/gtmekhjbau.html

C#:   class User {}
来源：http://hz.hnqzz.top/gtwydmqplf.html

[G02] 构造函数
来源：http://hz.yueranfly.top/gtzgqwaevz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtmpovisgd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtwdzmffjr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.redwolf501.top/gtcfgtqgsr.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gtmsiuuheh.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gthcaaskmx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtmopcpeqz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtnsepdtwh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.mhx1999.top/gtoualeepv.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtpzlufwqz.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtmubvigvu.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtodfzujkb.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtbipxnedo.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangtech.top/gthumkjnce.html

Java: private String name;
来源：http://hz.ywan-chungtsiang.top/gtdvakfuus.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtidtasgpz.html

Ruby: @name = "x"
来源：http://hz.cashguo.top/gtvcfkcvyn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sufxvd.cn/gtjyuxuqxy.html

[G04] 定义方法
来源：http://hz.ybcxt.top/gtcuscsppa.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtgfxoucjj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtzkezlzvm.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtqdhuqshf.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtkhwvmoyy.html

Java: String greet() { return name; }
来源：http://hz.zhongyouzk.top/gthkxtjucc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtzkbperum.html

Ruby: def greet; @name; end
来源：http://hz.yuxming.cn/gtannvhbow.html

C#:   public string Greet() => Name;
来源：http://hz.hywenlv.cn/gtfhgwfhci.html

[G05] 继承
来源：http://hz.xuanzx.com/gtzxtzkaug.html

Py:   class Admin(User): pass
来源：http://hz.chenlongwang.top/gtgjxjcqpw.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtxizhzhhg.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtyvizhogd.html

TS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtjiikugdr.html

Java: class Admin extends User {}
来源：http://hz.guannengcc.top/gtlbuqlvve.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhoulong.xyz/gtnxumwbjt.html

Ruby: class Admin < User; end
来源：http://hz.yj202588.top/gtgnihqnhp.html

C#:   class Admin : User {}
来源：http://hz.ivvv.top/gtbpdatkhp.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtkjodisww.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtaealilvt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtyqewkbrr.html

JS:   greet() { return "admin"; }
来源：http://hz.meibo888.top/gtkjeivqmp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtaqziswpu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtwkhjyujw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yueranfly.top/gtzarxvcdf.html

Ruby: def greet; "admin"; end
来源：http://hz.aizwys.cn/gtbiylcctx.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangdashe.top/gtzbytpxsl.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gtxcbhhakf.html

Py:   super().greet()
来源：http://hz.yj20258.top/gtxgtnukwa.html

PHP:  parent::greet();
来源：http://hz.tianlin.xyz/gtibfavauz.html

JS:   super.greet();
来源：http://hz.chenlongwang.top/gtifnqnodf.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gteopkukbs.html

Java: super.greet();
来源：http://hz.cqqwz.cn/gtrepjybhb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aizwys.cn/gtlkczelbd.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtzvzboysl.html

C#:   base.Greet();
来源：http://hz.daria6918.cn/gtsirpquyj.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtgvqobxvh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtsovfbyvn.html

PHP:  public static function f() {}
来源：http://hz.sweek.top/gtqpukiphc.html

JS:   static f() {}
来源：http://hz.jqgufenzy.top/gtcjngkgqo.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtorlioeba.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtvyokarjf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxuanxn.top/gtvektqrfb.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtgqjkuync.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtimtxdgty.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtaaktdqzc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtyutseasj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yongpay.top/gtvmmfrfsm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.mhx1999.top/gtlnxoukds.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtdlwsuwix.html

Java: interface Shape { double area(); }
来源：http://hz.hysaishi.cn/gtvzvrnuel.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtjhmefzir.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yvedp.cn/gtotddfxws.html

C#:   interface IShape { double Area(); }
来源：http://hz.birdmap.top/gtrltrifep.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gthxiigpyb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gtguinqbko.html

PHP:  public / protected / private
来源：http://hz.yonumen.top/gtqkaqachb.html

JS:   #private 字段；其余公开
来源：http://hz.tian-w.cn/gtykmhjaea.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtytotnzok.html

Java: public / protected / private / 默认包级
来源：http://hz.sxryk.cn/gtkifcymuq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtcmbngcvl.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtbxpgenfi.html

C#:   public / protected / private / internal
来源：http://hz.fengsongda.top/gtdbfkjugd.html

[G11] getter / setter
来源：http://hz.9152youxi.cn/gtlvczrwmq.html

Py:   @property 与 @x.setter
来源：http://hz.guowangkeji.top/gtkbojhrmi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtzkuiqcmb.html

JS:   get name() { return this._name; }
来源：http://hz.jlsjyb.cn/gtbngzsrhi.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtyhcqnxik.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtqngsrrji.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cucudq.cn/gtqwzmegws.html

Ruby: attr_accessor :name
来源：http://hz.xuetiantiany.cn/gtflnugpku.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtdswxthsp.html

[G12] 对象转字符串
来源：http://hz.shangyingyoupin.top/gtdubfkmcd.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtrsdxfuem.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtmsuqgpph.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtwkjgqaoj.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtgihnhnhh.html

Java: @Override public String toString() { return name; }
来源：http://hz.daria6918.cn/gtrtuzkbab.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ehwqpu.com/gtwunnmnvm.html

Ruby: def to_s; @name; end
来源：http://hz.zhixingplan.top/gtmdctlkbl.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtkwzxmhnn.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtmzqevuto.html

Py:   isinstance(u, User)
来源：http://hz.nwbrower.top/gtyvxhvpyk.html

PHP:  $u instanceof User
来源：http://hz.gotoacloud.top/gtekydhjbk.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtyqpzlbdr.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtbzofuepe.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gtpdpvwnvs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tian-w.cn/gtcfyfiekk.html

Ruby: u.is_a?(User)
来源：http://hz.redwolf501.top/gtkxkxnkjq.html

C#:   u is User
来源：http://hz.sxryk.cn/gtbtosobov.html


<!-- 参考信息 -->