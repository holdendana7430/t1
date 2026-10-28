代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hongshengwenyu.top/gtcvhsovhg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fengsongda.top/gtxyemhola.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ppjwa.cn/gtybsuhybn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dashuyun.cn/gtwguppjro.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtlvdsiwot.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtmsgydzjw.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtecyvhata.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gttqooopgw.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtzjewwenx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtphsrsulx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtkficbrfr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tianlin.xyz/gttyayiibo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.aizwys.cn/gtmtrihywv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtvutkjtvv.html

C#:   1234567.ToString("N0")
来源：http://hz.shuidangran.top/gtkstkfvue.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtwytzrrux.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jlsjyb.cn/gtbdiefipk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cqqwz.cn/gtfkjzafpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtcvgrddtb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtcilamkqo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.mhx1999.top/gteqtwsvim.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jianghu66.top/gtcjrzowrg.html

Ruby: s.capitalize
来源：http://hz.haohaochexian.top/gtkkzbolen.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258888.top/gtxyqbkswc.html

[E18] 模板占位符替换
来源：http://hz.0kj1m.cn/gtjbnurdkz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhijiandao.cn/gtcfvssymc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxuanxn.top/gtdinxhlnj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtrjxzogys.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtpgxnbegt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtotyxfvli.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daria6918.cn/gtzbhwzuji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gtmpyeeuab.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258.top/gtoivdmluv.html

[E19] 多行文本按行拆分
来源：http://hz.feifeiyinyue.top/gtuglzcoqn.html

Py:   s.splitlines()
来源：http://hz.havefunace.top/gtglitrhbi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gtsauwruxr.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtmxifcaxe.html

TS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtkdyrofnq.html

Java: s.lines().toList()
来源：http://hz.ydjk.org.cn/gtzrmbgqci.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gthffoycbw.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtpvqgumrm.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gttqvlwgic.html

[E20] 判断字符串是否为空
来源：http://hz.ppjwa.cn/gtmhfbhxvf.html

Py:   if not s:
来源：http://hz.hnxiangtu.top/gttiebumfh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtlpniqgux.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuanzhike.top/gtqfnbylhb.html

TS:   if (s === "") {}
来源：http://hz.zhiwuduotai.top/gtzbyqlubu.html

Java: if (s.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtwdimtjsc.html

Go:   if s == "" {}
来源：http://hz.fengsongda.top/gtntpuwtmf.html

Ruby: if s.empty?
来源：http://hz.yj202588.top/gtebbbupjd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.9152youxi.cn/gtfqzpgpby.html

[E21] 超长截断加省略号
来源：http://hz.zhiwuduotai.top/gtjgltjher.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cqqwz.cn/gtyxkzewzs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtfmpkotxu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtvkwibupu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtpnnwudxc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtlahunuzi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtpwasdivz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ybcxt.top/gtcnqfvbyw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtejufnwej.html

[E22] 字节长度与字符长度
来源：http://hz.aizwys.cn/gtvjndufsb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hongshengwenyu.top/gtaydmwdiy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtsccwyonq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtresqgcvt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtswdodqlg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gtsgrmftuy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigfzy.top/gtrkzkdsjb.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhiwuduotai.top/gtqqvrdiip.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shuidangran.top/gtmcfetxjx.html

================================================================================
来源：http://hz.gogol.net.cn/gthishygdb.html

F. 文件与目录
来源：http://hz.gaohongyu789.top/gtgstuoofh.html

================================================================================
来源：http://hz.nanxinkj.top/gtrthbhtrb.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtxrwiedma.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gtqzqcbkjt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hywenlv.cn/gthbkyeccm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jyoumei.cn/gtngxwljrj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtnqgxsdkp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtguuobfki.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gtcagthiwy.html

Ruby: File.read("a.txt")
来源：http://hz.nanxuanxn.top/gthonfgnlv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangdashe.top/gtzoexvytt.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtwxyuqukg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenzaomai.com/gtffgkpjvs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pengpengdd.cyou/gtqvxzvaqr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtibhtvjso.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtvckbxzns.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtcoyaohjw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gtvblyuopt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ehwqpu.com/gtjwqhnzgc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gtvjcnoklj.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtkpoitcha.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangkeji.top/gtspvwrnpv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtisyjedte.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtykpmkexs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtqaadhilc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtefyfwxcd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtnrjicdep.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.316326.xyz/gtrhnzdpxm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.c1oappe.top/gtwzexxnvo.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtgltywrbs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangtech.top/gtzaxzvkgw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtrjlkjydx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtpmuwlhzc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtxelodoet.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gttmtdboou.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gtzuynxdbq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gthpdsslun.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shzxlz.cn/gtfjmkgynx.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtfuphkfhb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gotoacloud.top/gtvkqsolik.html

PHP:  file_exists("a.txt");
来源：http://hz.yueranfly.top/gtjwxxhmcm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtzbnodmpp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtndyemkyi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtranmpgdo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhaomingkeji.xyz/gtwxeeqftv.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gthhebttvv.html

C#:   File.Exists("a.txt")
来源：http://hz.jlsjyb.cn/gtqpxmpjpj.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gtsopggsci.html

Py:   os.remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtuwzbugnt.html

PHP:  unlink("a.txt");
来源：http://hz.gzhubu.top/gtqcsaevhk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtonopxlfb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtmtctkhwy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtuiksiyhj.html

Go:   os.Remove("a.txt")
来源：http://hz.jiagoushi.top/gtyxouggxr.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtdmxqcqpt.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtyugknfom.html

[F07] 创建目录（含多级）
来源：http://hz.redwolf501.top/gtyacfhjzp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258.top/gtnzprkokh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sufxvd.cn/gtfrfhpmkb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtcgcbdyun.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gttlikolcq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yonumen.top/gtljengqbh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtjvghlbya.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aizwys.cn/gtaccuuivb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnqzz.top/gtvxfjgpxq.html

[F08] 遍历目录
来源：http://hz.zhoulong.xyz/gthecuakfu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gthuqrdqng.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gtooqfqtbb.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtltxrwfua.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtzfbmnysj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtalflbwzs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.316326.xyz/gtwufvrkat.html

Ruby: Dir.children("dir")
来源：http://hz.chenjidiqi.icu/gtckdkiyue.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtuslqpfxi.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtujehepxa.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtmjjyauep.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtmylvpbwa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtfdtjyydu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtkbqvcpto.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtpfaukplc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtfnheocsh.html

Ruby: File.size("a.txt")
来源：http://hz.tianlin.xyz/gtbhaaonjq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ppjwa.cn/gtyzvzcpck.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtfbmyjylg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtngpflqnj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtfpsdtaap.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtyybehmiw.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtltvvncdx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.redwolf501.top/gtlyumxhbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shzxlz.cn/gtkajwtbhh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtlqhsjfph.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gtseniqktm.html

[F11] 复制与移动文件
来源：http://hz.xingfuxueyuan.xyz/gtqefjmfct.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtebkibswp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuanzx.com/gtseljhxqp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtnowxxdze.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtabpigzgx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtpkhjdzen.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtlenjyeod.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtvitguosz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daria6918.cn/gtvdcrvgvr.html

[F12] CSV 读写
来源：http://hz.havefunace.top/gtrlbqjuen.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtilryxwlk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daria6918.cn/gtmsckfavh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtjjqbvqac.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtszsgwlmz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtbetvegtj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtwwnsuwyh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtcqkmqzxf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtesgmdiap.html

================================================================================
来源：http://hz.hammf.cn/gtmsopifjy.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtbiimyebj.html

================================================================================
来源：http://hz.xuanzx.com/gtbpstcgbw.html

[G01] 定义类
来源：http://hz.aibaodan.cn/gtyplfrgtk.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtusibzehh.html

PHP:  class User {}
来源：http://hz.fengsongda.top/gtqaqrlaqz.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtwevejycb.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gtefaeaaoy.html

Java: class User {}
来源：http://hz.hongshengwenyu.top/gtbyzardlh.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtvfjuvqth.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gtkxvupgzz.html

C#:   class User {}
来源：http://hz.kuanghao11.cn/gthttpvdnf.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gtqhanbtnu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtdeansqxf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zdqjudy.top/gttoefbrve.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtcfvniagh.html

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gtzipwoimh.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtgpcvukog.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtblypkvua.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cqqwz.cn/gtvsoehlfw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dianchejie.cn/gtegztthbd.html

[G03] 实例属性
来源：http://hz.316326.xyz/gtmhaocbif.html

Py:   self.name = "x"
来源：http://hz.yuanzhike.top/gtwjiinikl.html

PHP:  public string $name = "x";
来源：http://hz.redwolf501.top/gtomqulmtd.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtlbdsnltp.html

TS:   name: string = "x";
来源：http://hz.birdmap.top/gtrcrnsomn.html

Java: private String name;
来源：http://hz.yuanzhike.top/gtrxbxpkdb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtcgvhlaer.html

Ruby: @name = "x"
来源：http://hz.zhaomingkeji.xyz/gtptktgdgc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtmnvihdgy.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtevizzrcc.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtocyvctew.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtxnpjfpho.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtktnebgkd.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtgthbadbx.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtlqlndkts.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtgdtnrtxa.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtgjjvhuae.html

C#:   public string Greet() => Name;
来源：http://hz.tian-w.cn/gtkudfgzif.html

[G05] 继承
来源：http://hz.sweek.top/gtfsbxlhvz.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtpthdcyhn.html

PHP:  class Admin extends User {}
来源：http://hz.gogol.net.cn/gtqudzfleg.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtgzybmhxz.html

TS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtexuhejyn.html

Java: class Admin extends User {}
来源：http://hz.chenlongwang.top/gtcebvbzkl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.52xcode.cn/gtensjvhbe.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gtkwkjvfee.html

C#:   class Admin : User {}
来源：http://hz.9152youxi.cn/gtncucboux.html

[G06] 重写方法
来源：http://hz.jqgufenzy.top/gtctqbqhuw.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtyhywqdrj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtfkhlqlok.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtxwhzarux.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtjsopvzpb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtaazildzs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtinxsakru.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtmcoyhnms.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtjfphlzxi.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtrrzytvjo.html

Py:   super().greet()
来源：http://hz.birdmap.top/gtuolocwkk.html

PHP:  parent::greet();
来源：http://hz.jqgfzy.top/gtfsqmnluk.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtfxnfbknl.html

TS:   super.greet();
来源：http://hz.dianchejie.cn/gthgdgfbqs.html

Java: super.greet();
来源：http://hz.sufxvd.cn/gtyxmxibni.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shzxlz.cn/gtskndhozb.html

Ruby: super
来源：http://hz.fzhhl.top/gtgguiowob.html

C#:   base.Greet();
来源：http://hz.gogol.net.cn/gtocwbrpnd.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtzapwhtou.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zdqjudy.top/gtywfvirog.html

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gtbzvauiaj.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtvzyxvyvr.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtdbwimpto.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtrhlqnmyf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtaoglwmky.html

Ruby: def self.f; end
来源：http://hz.ydzc1.top/gtylggtiwv.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gtalztifnk.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258.top/gtrqbkosng.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenlongwang.top/gtdgsyznba.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtwlpnefsb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtfgacjdku.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtviqjlpwo.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtkraxdqth.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtelufbuuw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shangyingyoupin.top/gtbnjzqqyy.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtpnlsmchw.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gttfcdktlr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtaaccpfed.html

PHP:  public / protected / private
来源：http://hz.jlsjyb.cn/gtidrjtvae.html

JS:   #private 字段；其余公开
来源：http://hz.wangdashe.top/gtciubmwad.html

TS:   public / protected / private
来源：http://hz.wangshuangyany.cn/gtvwkmtefn.html

Java: public / protected / private / 默认包级
来源：http://hz.quarkkingdee.top/gtdzzdedgs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtxdpqusob.html

Ruby: public / protected / private
来源：http://hz.chenjidiqi.icu/gtarveslvo.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gthaxtzunq.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtxvicnysj.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gtirnjvyxw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtekycvlro.html

JS:   get name() { return this._name; }
来源：http://hz.dashuyun.cn/gtoixhmdxk.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtcxtzpopb.html

Java: public String getName() { return name; }
来源：http://hz.shangyingyoupin.top/gtsiqwsrhl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtdxsnzyhq.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtvjmjgewj.html

C#:   public string Name { get; set; }
来源：http://hz.fengsongda.top/gtapqvdbjg.html

[G12] 对象转字符串
来源：http://hz.mhx1999.top/gtirzitvjy.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtwiarmrqc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nwbrower.top/gteqxupgsd.html

JS:   toString() { return this.name; }
来源：http://hz.gotoacloud.top/gtmlvncrhx.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtblksgehz.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtgleqhnua.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtvjtetica.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtwjsdwnap.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gttelzrowj.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtvmaqjcli.html

Py:   isinstance(u, User)
来源：http://hz.hammf.cn/gtpdlqsbzw.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtnuuljubt.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gthpwvcota.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtsqmkzktl.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtuxmlpnzk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtnjnsbsha.html

Ruby: u.is_a?(User)
来源：http://hz.hnqzz.top/gtemlphwre.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtxuaxlocd.html


<!-- 参考信息 -->