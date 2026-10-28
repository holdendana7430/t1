代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtbpwgdynm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yongpay.top/gtkypxpkei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgfzy.top/gtnvuimmyr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aibaodan.cn/gtpcvdiisb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shangyingyoupin.top/gteusmpqdl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigfzy.top/gtcvyzctzd.html

[E16] 数字千分位
来源：http://hz.jqgufenzy.top/gtpjdznzej.html

Py:   f"{1234567:,}"
来源：http://hz.wangshuangyany.cn/gtafbmyxry.html

PHP:  number_format(1234567);
来源：http://hz.guowangkeji.top/gtekjfbwsj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtycalairw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtuuytacqp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gtthkwvwzh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gtplvayvvo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxinkj.top/gtlgeosqhu.html

C#:   1234567.ToString("N0")
来源：http://hz.ppjwa.cn/gtwfytupwo.html

[E17] 首字母大写
来源：http://hz.sxryk.cn/gthhrqizis.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zycfv.cn/gtcfspslgw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtfrbqqbrl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gtyezptgny.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gthalrmivh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gthxzkuewt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.snrcjt.cn/gtivzvbuiw.html

Ruby: s.capitalize
来源：http://hz.shuidangran.top/gtrwffegwb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuanzx.com/gtsjfosxcf.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtrvmbotrf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dashuyun.cn/gtxejtnvpc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sxryk.cn/gtxsjuxkca.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtdqmrghpa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtylxvucit.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zycfv.cn/gtnixgzecd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtjowbktwj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yvedp.cn/gthuolmrgz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtcuuwpvfk.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtaqsglkbc.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangkeji.top/gtrmflqjto.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fengsongda.top/gtqgpqbxuj.html

JS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtcwlpeymw.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtdpmnalmj.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtrrvhhlzb.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtggqxzmsp.html

Ruby: s.lines
来源：http://hz.cheryme.top/gtlytjunim.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtjmhdqqzm.html

[E20] 判断字符串是否为空
来源：http://hz.ydzc1.top/gtdknyyrqg.html

Py:   if not s:
来源：http://hz.gogol.net.cn/gtdqgsluam.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gtybbkerhr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gthsmuminx.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtnznbziut.html

Java: if (s.isEmpty()) {}
来源：http://hz.cheryme.top/gtlfcpkusi.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gtqcsxdqmf.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtpspczrgh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.wangdashe.top/gtbgnwypmp.html

[E21] 超长截断加省略号
来源：http://hz.chenlongwang.top/gtxkdhetiw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtylwnblvj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtnuauhlgv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtwxxnqlrj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtwionxcns.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtnfzrqgvs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daxiang520.top/gtfipmosdb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sysykeji.top/gtzjrrpoyp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtoychgkfr.html

[E22] 字节长度与字符长度
来源：http://hz.tianlin.xyz/gtxuiqmkgx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zdqjudy.top/gtezhmaxhi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtbubqmppw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtxxduepon.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtcumrpodl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yongpay.top/gtixdmrizq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gtacltiqpm.html

Ruby: s.bytesize;  s.length
来源：http://hz.ehwqpu.com/gtnumyqsmt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtsuppxrvi.html

================================================================================
来源：http://hz.ybcxt.top/gthsoqmpcq.html

F. 文件与目录
来源：http://hz.vqdsnc.cn/gtjexpbluw.html

================================================================================
来源：http://hz.guannengcc.top/gtnemeqejq.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtnmmxdmhw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtvcsnzrda.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtdikscwkz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.pengpengdd.cyou/gtidtavbow.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xziqi.cn/gtgdztxozn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtsnbrznwk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgufenzy.top/gtxjomvdhv.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gtutmepeqh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tianlin.xyz/gtjqxemaic.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtvmmogaxh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yanxiufei.cn/gtnmwqptqd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtjayvfyiv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtepcmtuce.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtqlweihnd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtwmsmumxs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.feifeiyinyue.top/gtbvznvscu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tian-w.cn/gtfqlyicug.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtyrvvmtlh.html

[F03] 写入文件（覆盖）
来源：http://hz.havefunace.top/gtgnmnfhsg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.52xcode.cn/gtnmrzzoyn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtwfgvgxop.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtjexkratd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtahblblzq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinyuanbaomall.cn/gtvfeosmht.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gtfntxgema.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxinkj.top/gtndhahuqu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pycfn.com/gtbvznpygo.html

[F04] 追加写入文件
来源：http://hz.jlsjyb.cn/gtkloepins.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.meibo888.top/gtsaydkvqx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtweytrptq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtpsfkxufw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtbsmfeqkt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ybcxt.top/gtevcedyof.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtrhhinmel.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yvedp.cn/gtafchgwrf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gzhubu.top/gtgmctagtk.html

[F05] 判断文件或目录是否存在
来源：http://hz.shuidangran.top/gtjfndbguv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuxming.cn/gtudmhfqkk.html

PHP:  file_exists("a.txt");
来源：http://hz.jinghuilouyu.cn/gtqztufugp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtwlnrkors.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtwaqdfdbb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtmozhdhym.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gtrcsnmujf.html

Ruby: File.exist?("a.txt")
来源：http://hz.zdqjudy.top/gtwanaituj.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtpkmcsydi.html

[F06] 删除文件
来源：http://hz.nanxuanxn.top/gtovuqcdfx.html

Py:   os.remove("a.txt")
来源：http://hz.cucudq.cn/gtahmszbsz.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gtkgnfulcb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtepoznppt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtzdspgqxq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtlqnfxsqo.html

Go:   os.Remove("a.txt")
来源：http://hz.sweek.top/gtclwwplob.html

Ruby: File.delete("a.txt")
来源：http://hz.zdqjudy.top/gtjasvetrs.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtfzopvusu.html

[F07] 创建目录（含多级）
来源：http://hz.smart0.xyz/gtudtjtojs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtuwrikjxm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxuanxn.top/gtflzsbgdl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtdahnogzn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gttknproqr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtftcwxlad.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtogtrcbdn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sufxvd.cn/gtbyzvcfyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtchakjhfj.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtaymbhkpu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtxwzhmica.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.9152youxi.cn/gtecfmonaa.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gttyixvzee.html

TS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtzwsmtqys.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shuidangran.top/gthvshorbu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.c1oappe.top/gtdbsbhxxl.html

Ruby: Dir.children("dir")
来源：http://hz.yongpay.top/gtihszvufb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.kuanghao11.cn/gtxaikdyks.html

[F09] 获取文件大小
来源：http://hz.9152youxi.cn/gtupotrwdz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtqpkmrlms.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtfaohwjlx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtjyvdumnz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gtdchvdoqt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtrshhzchc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenzaomai.com/gtiawoydna.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtxcefcgxg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenlongwang.top/gtzdmedxji.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhiwuduotai.top/gtoljukhre.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtbpvadtas.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gtdonmjwmg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtltsgbcwm.html

TS:   path.extname("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtspagkppe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hongshengwenyu.top/gtpaiqmwyc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtvffrxmiq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtyqusjrti.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydzc1.top/gtbskvmhrn.html

[F11] 复制与移动文件
来源：http://hz.xylfe.cn/gtahaemzve.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gttdjibsdm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gtelixbjth.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gthnxktnhn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtaqqaxwkg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.meibo888.top/gtjrfyaxwu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gteagtfege.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtvrgnhzln.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sxryk.cn/gtgmxqlage.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtsgsrynee.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hfpthk.cn/gtcxickply.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.meibo888.top/gtxydlekja.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj202588.top/gtfpufpbmm.html

TS:   // 同上
来源：http://hz.ppjwa.cn/gtlmsclwyf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zdqjudy.top/gtrbotoeof.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gthqlqqohg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gtpbodtxzy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dashuyun.cn/gttaclwtmg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtthrmvcbs.html

G. 面向对象
来源：http://hz.gzhubu.top/gtdlcbhvel.html

================================================================================
来源：http://hz.sufxvd.cn/gtykjtzsjz.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtzacuctbh.html

Py:   class User: pass
来源：http://hz.chenjidiqi.icu/gtyslcxtzc.html

PHP:  class User {}
来源：http://hz.kuanghao11.cn/gtyzsggkik.html

JS:   class User {}
来源：http://hz.tian-w.cn/gtabyxdxbn.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gtwzumklay.html

Java: class User {}
来源：http://hz.xylfe.cn/gtftvppzkh.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtueloubxu.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gthdwgzafx.html

C#:   class User {}
来源：http://hz.ydzc1.top/gtsgexjair.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtavgmxnxh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jlsjyb.cn/gtkfmqeyev.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.c1oappe.top/gtndchuxdk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtwktofupb.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtymrxfxpq.html

Java: User(String name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtrrogubuh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtjnzypsxr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtqtgdophf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtpynxpkcd.html

[G03] 实例属性
来源：http://hz.birdmap.top/gtkfdtgggs.html

Py:   self.name = "x"
来源：http://hz.havefunace.top/gtuqpvgixp.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gttouxlpuw.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtvknlqoyi.html

TS:   name: string = "x";
来源：http://hz.jinqigfzy.top/gtuafxhbsz.html

Java: private String name;
来源：http://hz.guowangkeji.top/gtndoyilzb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fengsongda.top/gtomcijfdq.html

Ruby: @name = "x"
来源：http://hz.c1oappe.top/gtlgnygnyo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cashguo.top/gtehxsnlam.html

[G04] 定义方法
来源：http://hz.sweek.top/gtfcvymcpb.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtfzbhbtwu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtmvsblbio.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gtccpvjbwe.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gttesuqqpv.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtzqxxduff.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gthfhpjund.html

Ruby: def greet; @name; end
来源：http://hz.vqdsnc.cn/gtpibxehvh.html

C#:   public string Greet() => Name;
来源：http://hz.ybcxt.top/gtffsmnrwh.html

[G05] 继承
来源：http://hz.hywenlv.cn/gtxhlddogm.html

Py:   class Admin(User): pass
来源：http://hz.zhaomingkeji.xyz/gtoxnvehgf.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtwpahleuy.html

JS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtdsjxkgjx.html

TS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtuusskcqa.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtdsknbkjp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.guannengcc.top/gtewdqbxqk.html

Ruby: class Admin < User; end
来源：http://hz.feifeiyinyue.top/gtqnzesiqn.html

C#:   class Admin : User {}
来源：http://hz.chenlongwang.top/gtealjualr.html

[G06] 重写方法
来源：http://hz.meibo888.top/gttlrdwhee.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtcigoftwe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gttjxsvoph.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtlqrbvhjx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtpawhgcig.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtomsxhwqb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtzljwyuci.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtycpzbapv.html

C#:   public override string Greet() => "admin";
来源：http://hz.daxiang520.top/gtvgstanis.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtufczisuo.html

Py:   super().greet()
来源：http://hz.yvedp.cn/gtkcvlkrhs.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtmahtmvxz.html

JS:   super.greet();
来源：http://hz.gogol.net.cn/gtjacndqxh.html

TS:   super.greet();
来源：http://hz.cheryme.top/gtjlpwfxot.html

Java: super.greet();
来源：http://hz.316326.xyz/gtvryxlrbm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxuanxn.top/gtyxgosaac.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtfsztucpv.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtukuoypif.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtjoxnawhe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nwbrower.top/gtybtkvetl.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtmympfdtk.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtreuhggcn.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtjnlqnloe.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtogikasuq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtakbtmplu.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtvqcbxlpj.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtjoftnnak.html

[G09] 接口 / 抽象类
来源：http://hz.mhx1999.top/gtojfxynng.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtjwxczljj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zycfv.cn/gtpnqjwkcy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gtgwbpfpol.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gtyymxflil.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gtjnncmsva.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtzftlplbh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtwpvarmep.html

C#:   interface IShape { double Area(); }
来源：http://hz.aibaodan.cn/gtppamwmuv.html

[G10] 访问控制
来源：http://hz.cheryme.top/gtyhjkcvos.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ehwqpu.com/gtcrzefxna.html

PHP:  public / protected / private
来源：http://hz.ehwqpu.com/gttontzqje.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258888.top/gteewbkttq.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtyjdoezop.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtgeqkqxaz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cheryme.top/gtxuhsahbs.html

Ruby: public / protected / private
来源：http://hz.gogol.net.cn/gtmtgjyncl.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtawomelpj.html

[G11] getter / setter
来源：http://hz.meibo888.top/gtkyerejdw.html

Py:   @property 与 @x.setter
来源：http://hz.hysaishi.cn/gtejrioyuk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtitvdzzzr.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gteschyfpv.html

TS:   get name(): string { return this._name; }
来源：http://hz.jyoumei.cn/gtgwadxall.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtumiwfimp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtobscqgyv.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtnrjnuxiy.html

C#:   public string Name { get; set; }
来源：http://hz.jinghuilouyu.cn/gtxqwwtjug.html

[G12] 对象转字符串
来源：http://hz.shangyingyoupin.top/gtxousweur.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtlrjnpfru.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtkkygqjkx.html

JS:   toString() { return this.name; }
来源：http://hz.svipenyu.cn/gtgmvohqjn.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gttimsouaa.html

Java: @Override public String toString() { return name; }
来源：http://hz.birdmap.top/gtrrejyguy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cdnleiting.top/gtqgrsijlz.html

Ruby: def to_s; @name; end
来源：http://hz.sufxvd.cn/gterlejhvs.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtbclmzskq.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gtzznwjnsk.html

Py:   isinstance(u, User)
来源：http://hz.hysaishi.cn/gtqalglwjr.html

PHP:  $u instanceof User
来源：http://hz.yj20258888.top/gtnmewcvpj.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtfecswtuy.html

TS:   u instanceof User
来源：http://hz.chenlongwang.top/gtusaeeaqm.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtiynzoomh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tian-w.cn/gtljkkqhmh.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtgkckuuzf.html

C#:   u is User
来源：http://hz.tanke756.top/gtdloatbcv.html


<!-- 参考信息 -->