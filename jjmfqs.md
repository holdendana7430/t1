代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pycfn.com/gtuayucnbp.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigufen.top/gtvljbvkue.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dashuyun.cn/gtovbmkrgz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.fzhhl.top/gtzqshqgvc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hongshengwenyu.top/gttuxsjdqw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gtfcbykuas.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.snrcjt.cn/gtenbsjqnt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xinyue.icu/gtzstmejne.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cdnleiting.top/gtjaayzura.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtggkvoeug.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtzlxjrtdm.html

Py:   f"{1234567:,}"
来源：http://hz.kuanghao11.cn/gtzzmiljcp.html

PHP:  number_format(1234567);
来源：http://hz.ybcxt.top/gtmowudckc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtcucvoiyz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gtplqblfzu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhiwuduotai.top/gtrxsbxhkh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtpviadqjt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xuetiantiany.cn/gtlkllawlj.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtdgwpfndh.html

[E17] 首字母大写
来源：http://hz.jinqigufen.top/gtrbpgnlne.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shangyingyoupin.top/gtothpncsu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtpiaaxhae.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtkxqynlro.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gthzownhzj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fengsongda.top/gtezcvpyas.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.9152youxi.cn/gtioqnmxss.html

Ruby: s.capitalize
来源：http://hz.zycfv.cn/gtkjyuoxlt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtbtdnytvu.html

[E18] 模板占位符替换
来源：http://hz.0kj1m.cn/gtfaplgsep.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cheryme.top/gtnpxzmgtl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtxohzndbj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtwzkhpqbn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gthvrnidyn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gteneyznvc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtvzolqgly.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtydwjcnrc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yangfankeji.com/gtgnbvktsl.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtjvnihsgo.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtzhyajujh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ppjwa.cn/gtndrtgmht.html

JS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtubfmwlhc.html

TS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gticdosphf.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtwwsyllxm.html

Go:   strings.Split(s, "\n")
来源：http://hz.gzhubu.top/gtzpacrksu.html

Ruby: s.lines
来源：http://hz.yongpay.top/gtkedqkmki.html

C#:   s.Split('\n')
来源：http://hz.chenlongwang.top/gtshumhbus.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtedlcbqog.html

Py:   if not s:
来源：http://hz.52xcode.cn/gtccbbinsq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtjxiivhip.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtwkgsqwig.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtqrhibrqx.html

Java: if (s.isEmpty()) {}
来源：http://hz.cheryme.top/gtlngnzuxc.html

Go:   if s == "" {}
来源：http://hz.hysaishi.cn/gtbwomkdbm.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gtawayekds.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xinyue.icu/gtnrlaquqi.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtwptmqbvf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tianlin.xyz/gtyrzerqhg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.svipenyu.cn/gtehcogrtq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtylfguzqk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtuntmokls.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtavfcxptw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtuaelowfq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigufen.top/gttzvfltmu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuanzhike.top/gtibtcwkvh.html

[E22] 字节长度与字符长度
来源：http://hz.jyoumei.cn/gtshvmwley.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xylfe.cn/gtmbsnqteh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtnhfhrnvu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtemdrennf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtpkgynopi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xziqi.cn/gtextajkei.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtijmzhcbo.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gthnzyqtoq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuxming.cn/gtiadcayjf.html

================================================================================
来源：http://hz.hnqzz.top/gtenvayukg.html

F. 文件与目录
来源：http://hz.jinghuilouyu.cn/gtjgxgauum.html

================================================================================
来源：http://hz.hywenlv.cn/gtbrwquzvc.html

[F01] 读取整个文件
来源：http://hz.chenjidiqi.icu/gtsimqockd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtanbcjqgt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gthvboyson.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gtqafcuoaz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.0kj1m.cn/gtbwiglqea.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtefcqdyzs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shzxlz.cn/gtnkgfelvk.html

Ruby: File.read("a.txt")
来源：http://hz.jinghuilouyu.cn/gtqtqniltg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tian-w.cn/gtgbiqqvyl.html

[F02] 逐行读取文件
来源：http://hz.nanxinkj.top/gtywqsluzv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nwbrower.top/gtxpqsasue.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtiwgjpvhh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtnbzkdjlm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gttfvptwlp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtamkprbys.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aizwys.cn/gtjclmdldt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtbrxcpzvr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtgzhvdrac.html

[F03] 写入文件（覆盖）
来源：http://hz.sufxvd.cn/gtzjaebkks.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ppjwa.cn/gtvxbzptfj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.c1oappe.top/gtjyvljrzk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtuzarqvdx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtabbpqdls.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtfhboddpr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangtech.top/gtnwoatzvk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.316326.xyz/gtolovfuja.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cashguo.top/gtbuqrhzie.html

[F04] 追加写入文件
来源：http://hz.zdqjudy.top/gtwfsrrdrz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tian-w.cn/gttqjrknhu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cdnleiting.top/gtmicvrghr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtkbzubqrk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtevaxdrgn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aizwys.cn/gtjvxrjkfc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.0kj1m.cn/gtbijvnram.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shuidangran.top/gtjzhdneev.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtyalmwrsw.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gtnkvbewhm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shangyingyoupin.top/gtjsyfiumg.html

PHP:  file_exists("a.txt");
来源：http://hz.havefunace.top/gtpahyemmy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtdueoazxh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtenfpyuns.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtldhrmijt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yongpay.top/gtnjbgionx.html

Ruby: File.exist?("a.txt")
来源：http://hz.cdnleiting.top/gtaotopywd.html

C#:   File.Exists("a.txt")
来源：http://hz.redwolf501.top/gtgyawekwj.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtjkherklt.html

Py:   os.remove("a.txt")
来源：http://hz.yuanzhike.top/gtqtnucqcu.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gtxjggpjfx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtavzagbfs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtrmiehqix.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtkcknsqxi.html

Go:   os.Remove("a.txt")
来源：http://hz.meibo888.top/gtqbagpdmq.html

Ruby: File.delete("a.txt")
来源：http://hz.yj202588.top/gtznmgqcrj.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gtdxnulwun.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtyxlzrufw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtaebcttet.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhongyouzk.top/gtpbibyrcf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtnjvtoisg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtjdtjslmn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jyoumei.cn/gtdwzjnbfn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtoxrpgkbw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtpgqozrcs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258.top/gtxclzzqnw.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtuchhiwol.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtuwanwswb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtpuvvxozd.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtqecggeno.html

TS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtzprupfpr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtfonkkzyz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtypztraut.html

Ruby: Dir.children("dir")
来源：http://hz.nanxuanxn.top/gtlacbwxtt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shuidangran.top/gtuichvwtt.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtkvrsyofk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hysaishi.cn/gtlklgkevd.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gthtoszoxp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtjdwoqsjv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtbdcmpepl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtvwbpsuat.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gttipkaizs.html

Ruby: File.size("a.txt")
来源：http://hz.chenlongwang.top/gtjewfrvkz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gtpmgbilqm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ehwqpu.com/gtpnnwwqty.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtghjbjzsj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.birdmap.top/gtiaktqlza.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtavcadwoh.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtfrwxsbpg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigfzy.top/gtrrwcqlov.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtmgspwqje.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtqeavqvbw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuanzhike.top/gtxnfncfsz.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtgphvydor.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtdsbaxrfy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.iojbl.cn/gtxdvtsvht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gttgacmmkk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtletznyxz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guowangkeji.top/gtnbwftlni.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtkevqvxrm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtawjnvvyx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtehkngdvk.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gtzchojyke.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fengsongda.top/gtnobxhdjd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gtvwzoshfz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yongpay.top/gtggvdqbrz.html

TS:   // 同上
来源：http://hz.shuidangran.top/gtgeyklhph.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtscvtwivr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtxcablqmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.dashuyun.cn/gtwhjaaxeg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtndcratxo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtzcojyocf.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtunyvfqej.html

================================================================================
来源：http://hz.9152youxi.cn/gtxukqmdol.html

[G01] 定义类
来源：http://hz.yj20258.top/gtbswyiukr.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtvrjfsogm.html

PHP:  class User {}
来源：http://hz.ydjk.org.cn/gthyofuwpv.html

JS:   class User {}
来源：http://hz.c1oappe.top/gtlhubanmw.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgfzy.top/gtsffssnur.html

Java: class User {}
来源：http://hz.cqqwz.cn/gtufdrjayq.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtuaoetssx.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtsrhixshn.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtyijgyipi.html

[G02] 构造函数
来源：http://hz.meibo888.top/gtmzcdtjev.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtsggctrjz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtcesxmcsa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtqhskjjou.html

TS:   constructor(public name: string) {}
来源：http://hz.cqqwz.cn/gtpradptel.html

Java: User(String name) { this.name = name; }
来源：http://hz.jiagoushi.top/gthxymwmyh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtugaxneov.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtrpzaoend.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtianaukhz.html

[G03] 实例属性
来源：http://hz.nwbrower.top/gtguiwywjj.html

Py:   self.name = "x"
来源：http://hz.daxiang520.top/gtuvssybqr.html

PHP:  public string $name = "x";
来源：http://hz.jinyuanbaomall.cn/gtivvtjcxd.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtgqeddbmu.html

TS:   name: string = "x";
来源：http://hz.fengsongda.top/gtyvtiwywm.html

Java: private String name;
来源：http://hz.0kj1m.cn/gtyhokkrxs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gttxashhui.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtkopcgovz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gtqwoakcsn.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gthmpqlqek.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtwwnwvznu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtgahckrlb.html

JS:   greet() { return this.name; }
来源：http://hz.iojbl.cn/gtdbrobznf.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtprfmsqcs.html

Java: String greet() { return name; }
来源：http://hz.ydzc1.top/gtawunnlje.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtrrogggwg.html

Ruby: def greet; @name; end
来源：http://hz.zdqjudy.top/gtobxwevtx.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtiwajdxvk.html

[G05] 继承
来源：http://hz.svipenyu.cn/gtbnemokxx.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtkozuqdbz.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtszgpzysz.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtomddavup.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtgtonxtsm.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtddqvkwyg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinyuanbaomall.cn/gthducncgn.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtosnakdqc.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gttrsgiilt.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtbwicqcvk.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtmyhzopbt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtphykapao.html

JS:   greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtmjxfshvw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtckxyesgw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gthwxkpiwr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gotoacloud.top/gtyoaegfpf.html

Ruby: def greet; "admin"; end
来源：http://hz.gogol.net.cn/gtdwwysmzn.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtzygvhoab.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtyyhdqjvw.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtqordecoe.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtfseqolhq.html

JS:   super.greet();
来源：http://hz.chenlongwang.top/gtakjtkrdq.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtjsttjarv.html

Java: super.greet();
来源：http://hz.zdqjudy.top/gtbkdqodtp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtxugdqfio.html

Ruby: super
来源：http://hz.yonumen.top/gtaaaapfbv.html

C#:   base.Greet();
来源：http://hz.ydzc1.top/gtmiuiibyw.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtnjrpqujz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtvpljgion.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gttgxkcnnc.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtqmyysbfu.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtgwocujvi.html

Java: static void f() {}
来源：http://hz.sysykeji.top/gtrcmjxpps.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtvjnmlsfq.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtkchakavv.html

C#:   public static void F() {}
来源：http://hz.yj202588.top/gtunaxjqie.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtbbqzycms.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jianghu66.top/gtogdokcen.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtkronvgrb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aibaodan.cn/gtgbitjorc.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gtqwhswvbm.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtqezfkqsy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gtjrowuhda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtaucdskuk.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtivqdbgwo.html

[G10] 访问控制
来源：http://hz.gotoacloud.top/gtiupjvmqb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtetletkth.html

PHP:  public / protected / private
来源：http://hz.shuidangran.top/gtkcnzhrmh.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtvlmtqswd.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtkvnabouv.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gthnhluryo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hywenlv.cn/gtkmdliouf.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gtcglosytq.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtiwgzvmud.html

[G11] getter / setter
来源：http://hz.hnqzz.top/gtfzkauurd.html

Py:   @property 与 @x.setter
来源：http://hz.guowangkeji.top/gtbhvbioiy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtvnqcswcu.html

JS:   get name() { return this._name; }
来源：http://hz.jqgufenzy.top/gtkbbswqou.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtpyyedujs.html

Java: public String getName() { return name; }
来源：http://hz.gzhubu.top/gtylrntufg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtjvmybogq.html

Ruby: attr_accessor :name
来源：http://hz.0kj1m.cn/gtgcmmjtse.html

C#:   public string Name { get; set; }
来源：http://hz.daxiang520.top/gtriicooge.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gthpufyige.html

Py:   def __str__(self): return self.name
来源：http://hz.yvedp.cn/gtyibbsauk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj202588.top/gtpjjexupr.html

JS:   toString() { return this.name; }
来源：http://hz.cucudq.cn/gtldalbecp.html

TS:   toString(): string { return this.name; }
来源：http://hz.xinyue.icu/gtuegmykgv.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenlongwang.top/gtnjteeucq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sysykeji.top/gtvypppjvs.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtmbejaujz.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gttootlxcp.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtzkfndccf.html

Py:   isinstance(u, User)
来源：http://hz.nwbrower.top/gtdhugiqvg.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtqyqxixjs.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtwlmwirrm.html

TS:   u instanceof User
来源：http://hz.jinqigufen.top/gtpgdftrex.html


<!-- 参考信息 -->