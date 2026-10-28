代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sxryk.cn/gtfglxzhrb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gteadmkjzu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhiwuduotai.top/gtspkcmakz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hongshengwenyu.top/gtpnwqcblc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cucudq.cn/gtjpsdfkaz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gogol.net.cn/gtdikmkwdc.html

[E16] 数字千分位
来源：http://hz.cheryme.top/gtqpygdvea.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtjigyluep.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtsbvhyrbr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtvefkwxuc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtvzjqymlk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gzhubu.top/gtftcypunj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ppjwa.cn/gtbmzrxbcm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangdashe.top/gtayotldcj.html

C#:   1234567.ToString("N0")
来源：http://hz.xuanzx.com/gtckkjixfb.html

[E17] 首字母大写
来源：http://hz.zhiwuduotai.top/gtbqkfibdd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xinyue.icu/gtcwztegnq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinghuilouyu.cn/gtawvdbipv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtqborrsrc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtluuamvvr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenzaomai.com/gtodqypywi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.c1oappe.top/gtkueiyezb.html

Ruby: s.capitalize
来源：http://hz.yongpay.top/gtbaxbqwqc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtsgitnzvl.html

[E18] 模板占位符替换
来源：http://hz.sweek.top/gtueoygvah.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.andypj.xyz/gtpugutvel.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhijiandao.cn/gtiphkquqf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtcihenolj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtwbcjeibq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.birdmap.top/gtmqaaseof.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhijiandao.cn/gttftjcfxj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtgvadbxbp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.meibo888.top/gtinwnwzge.html

[E19] 多行文本按行拆分
来源：http://hz.pycfn.com/gtwzzcevej.html

Py:   s.splitlines()
来源：http://hz.yonumen.top/gtcbvvytpf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gtqspjonuu.html

JS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtlhjaduhl.html

TS:   s.split(/\r?\n/)
来源：http://hz.gzhubu.top/gtqkdecemq.html

Java: s.lines().toList()
来源：http://hz.zhongyouzk.top/gtpcgxfxpk.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuanzx.com/gtvmivtyri.html

Ruby: s.lines
来源：http://hz.iojbl.cn/gtgtfhhqxl.html

C#:   s.Split('\n')
来源：http://hz.jianghu66.top/gtlfvuifml.html

[E20] 判断字符串是否为空
来源：http://hz.cucudq.cn/gtbxotovog.html

Py:   if not s:
来源：http://hz.aizwys.cn/gtnqaumzce.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgufenzy.top/gtaggbzetw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydjk.org.cn/gtwrtwhfuv.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gtwtykwkbo.html

Java: if (s.isEmpty()) {}
来源：http://hz.hysaishi.cn/gthbsmbwpp.html

Go:   if s == "" {}
来源：http://hz.aizwys.cn/gtvalcqwbz.html

Ruby: if s.empty?
来源：http://hz.daria6918.cn/gtmczdulmp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangkeji.top/gttjltoluy.html

[E21] 超长截断加省略号
来源：http://hz.yonumen.top/gtjyngmovv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtorovisxs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.quarkkingdee.top/gtgxyexnyq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtfhpclkov.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtlmgvheah.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtfoyiddgw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtoklnzvqc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ybcxt.top/gthqdsrqqe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zdqjudy.top/gtxltjrrjj.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtqlonmjih.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtkfgozxcs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtforfbjoy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gthxhlexul.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtjnzcfmnr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.meibo888.top/gtwrwupjrb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xziqi.cn/gtyqwqsdfy.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtabxhhbsr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtxmqyvzlv.html

================================================================================
来源：http://hz.fzhhl.top/gtuxnimltt.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtgucepded.html

================================================================================
来源：http://hz.yonumen.top/gtsqldfrch.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtzwhkmwxf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtuslopkap.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gtnvnqwwds.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xingfuxueyuan.xyz/gtjncyjopd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtabzqxkns.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtzjfqnyto.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.havefunace.top/gtdvuaimxb.html

Ruby: File.read("a.txt")
来源：http://hz.52xcode.cn/gtxhmkgupl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tian-w.cn/gtrcjzidet.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtfjadjzei.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuetiantiany.cn/gtgqvldzne.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtmtyagsdp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.quarkkingdee.top/gtifioryho.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtrufpuctm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtkgiavxbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtttwrsrcn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.redwolf501.top/gtjakevgeo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.feifeiyinyue.top/gtigxutnem.html

[F03] 写入文件（覆盖）
来源：http://hz.sysykeji.top/gteopewpce.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xingfuxueyuan.xyz/gtmjtjzops.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtscgimbiv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtqllcnwgk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtrtkyjekc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pycfn.com/gtoaxwimpm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.9152youxi.cn/gtmsdofgjv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shuidangran.top/gtevbwydwm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtaabgkvbh.html

[F04] 追加写入文件
来源：http://hz.snrcjt.cn/gtlfdiecnp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gtagseyorx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gttzfnsvfl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gthwsjhkwj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangshuangyany.cn/gtvhnabroc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhijiandao.cn/gtwfuzuzrd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtpfauqmhq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtqaeulbgh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gthpevnuiy.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgfzy.top/gtkxswyftm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtneevclht.html

PHP:  file_exists("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtxloqloac.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gtbunooqvr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtandvnypg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtccnyixba.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gogol.net.cn/gtrkuvgoww.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenlongwang.top/gtwxcpagte.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtyaqqxouw.html

[F06] 删除文件
来源：http://hz.shzxlz.cn/gtegdtsnqu.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtmjlgeryn.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gthdedtgkv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtknyxjffr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtzlmmrlrg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtgyykndra.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtyeeteook.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtnavjfmhz.html

C#:   File.Delete("a.txt");
来源：http://hz.tianlin.xyz/gtsaoulfck.html

[F07] 创建目录（含多级）
来源：http://hz.yonumen.top/gtdolwrwfx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtivssrowt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shuidangran.top/gtskqvwgig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtkvtmlhwc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtphtlmono.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.mhx1999.top/gtwrcjtmip.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.andypj.xyz/gtvwetxois.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhaomingkeji.xyz/gtyessjsmg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.bjfxy.top/gtdpqirgee.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gtbldboney.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hywenlv.cn/gtfdntcfql.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtcgvmwxnm.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtlmjsosfi.html

TS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtwvttenyr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtnksdbkww.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gtiiruzoeg.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtwlxjypwz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtmehmajis.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtqqulouzb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigfzy.top/gtcmcoutyc.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtfqqrzgrh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtiihntawc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtoolukivh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtloyrjbjz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtbuxhegjn.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtlbidzzna.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtqxlajxqt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cqqwz.cn/gtigmdebpv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtggxnmifn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtneedarqw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtupvyopwl.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtzxyqhotz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtezjjdmze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dianchejie.cn/gtlxbcxmei.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtajklkxjj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gthpkftryw.html

[F11] 复制与移动文件
来源：http://hz.jqgufenzy.top/gtpfpmezkv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtzuxabgne.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.c1oappe.top/gtikalhass.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtxwedtzaj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtliianlra.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gtkinopcyx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gtokxbnukw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtxvycoatl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jianghu66.top/gtbytmsmjw.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gtzjtoiakn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.svipenyu.cn/gtyxrezmuf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtmttbfunr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtvzyizrqp.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtpgunwuid.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gtvswlguhl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.snrcjt.cn/gtavrbwurr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtlcbuyyfm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhengqikj.top/gtspnoqvjr.html

================================================================================
来源：http://hz.snrcjt.cn/gtvimczuwe.html

G. 面向对象
来源：http://hz.xziqi.cn/gtvnclqmjw.html

================================================================================
来源：http://hz.tanke756.top/gtidgpcpht.html

[G01] 定义类
来源：http://hz.hammf.cn/gtckpvckkx.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtvmtirbxj.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtplweeoce.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtygsnxrwn.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtfuplmfqb.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtpxyctsok.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtvbwiysoh.html

Ruby: class User; end
来源：http://hz.jianghu66.top/gtknczywld.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtsznqfncf.html

[G02] 构造函数
来源：http://hz.cucudq.cn/gtqanaiyrf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ehwqpu.com/gtwtmxmwbd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtrnbrimvm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtgmlavgxs.html

TS:   constructor(public name: string) {}
来源：http://hz.shuidangran.top/gtrjuvorbj.html

Java: User(String name) { this.name = name; }
来源：http://hz.shuidangran.top/gtzcsncbyt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtpyjhayzd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.kuanghao11.cn/gtdhycdeyj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gttaiqjwre.html

[G03] 实例属性
来源：http://hz.smart0.xyz/gtoyfkemli.html

Py:   self.name = "x"
来源：http://hz.zhijiandao.cn/gtenbnfmam.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gtwfjnsxpo.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtkcdcgjkm.html

TS:   name: string = "x";
来源：http://hz.ywan-chungtsiang.top/gtwkigauez.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtxvfphrlt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuanzhike.top/gtapbyvyyy.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtwmapghtz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xziqi.cn/gtgbkurmwk.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtjewmdlkl.html

Py:   def greet(self): return self.name
来源：http://hz.cqqwz.cn/gtujpfomlm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtbfwohumi.html

JS:   greet() { return this.name; }
来源：http://hz.sweek.top/gtzphoppyx.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtwbptyjlh.html

Java: String greet() { return name; }
来源：http://hz.jinghuilouyu.cn/gtpvytguso.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtebkjhosh.html

Ruby: def greet; @name; end
来源：http://hz.sxryk.cn/gtpzqmlrvb.html

C#:   public string Greet() => Name;
来源：http://hz.gaohongyu789.top/gtxszgslfh.html

[G05] 继承
来源：http://hz.shanyushiyangtech.top/gtpwubojoa.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gtljrpmzkb.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtuedpwntm.html

JS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gteffhosel.html

TS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtohiauzxz.html

Java: class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtnykehlgp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gtrrjadfda.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtzfprfobf.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtozlldnjn.html

[G06] 重写方法
来源：http://hz.316326.xyz/gtwjvwjhne.html

Py:   def greet(self): return "admin"
来源：http://hz.dashuyun.cn/gtpzmvbnoh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtsniigdog.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtxzcydeec.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtqxspuavr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtgzqdfoge.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxuanxn.top/gtnavfhvvy.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtngxjakku.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtlolzitrp.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtvkugpcnn.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtlvmjqjkl.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gtidrcehug.html

JS:   super.greet();
来源：http://hz.dianchejie.cn/gtfetcgbmf.html

TS:   super.greet();
来源：http://hz.guannengcc.top/gtisklzerx.html

Java: super.greet();
来源：http://hz.smart0.xyz/gtoffmlcvr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtbsyjedqu.html

Ruby: super
来源：http://hz.zycfv.cn/gtvzprokef.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtfhqhxsny.html

[G08] 静态方法与属性
来源：http://hz.yvedp.cn/gtttomasvt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangkeji.top/gtgrwqfjge.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtpmawncur.html

JS:   static f() {}
来源：http://hz.0kj1m.cn/gtfgovvgdi.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtmskqovja.html

Java: static void f() {}
来源：http://hz.316326.xyz/gtpidenvyr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtsbrrexyy.html

Ruby: def self.f; end
来源：http://hz.daria6918.cn/gtzsimiwio.html

C#:   public static void F() {}
来源：http://hz.zhengqikj.top/gtyvaojemv.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtaqwwixnu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gtrogjhklo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ybcxt.top/gtobhkgiok.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtvkfzpxes.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtjngsqlkn.html

Java: interface Shape { double area(); }
来源：http://hz.jlsjyb.cn/gtdennbtpk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtcfpnhlhh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtmnqschpe.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtrifbzycf.html

[G10] 访问控制
来源：http://hz.jinyuanbaomall.cn/gtzpucgvsz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydzc1.top/gtqgabledm.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtxoudqjap.html

JS:   #private 字段；其余公开
来源：http://hz.hywenlv.cn/gttkbxwyjx.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gttzzkhcxy.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gttfbizfgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtcibsmlhx.html

Ruby: public / protected / private
来源：http://hz.yuanzhike.top/gtlreoblfo.html

C#:   public / protected / private / internal
来源：http://hz.andypj.xyz/gtqalwodae.html

[G11] getter / setter
来源：http://hz.sufxvd.cn/gtxbskiaxe.html

Py:   @property 与 @x.setter
来源：http://hz.ppjwa.cn/gtdchsprnk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtxfhhxhpm.html

JS:   get name() { return this._name; }
来源：http://hz.cashguo.top/gtvmjqzamp.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtwjpykusu.html

Java: public String getName() { return name; }
来源：http://hz.c1oappe.top/gtswmvsaud.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gttayznfyd.html

Ruby: attr_accessor :name
来源：http://hz.birdmap.top/gtfasngnog.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtlvhghske.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtbpzuwibj.html

Py:   def __str__(self): return self.name
来源：http://hz.dianchejie.cn/gtsdyotceb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtrqowmcsd.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtbcywjkfk.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtehrebutp.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigfzy.top/gtvahsbvap.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gttzvuwhov.html

Ruby: def to_s; @name; end
来源：http://hz.yueranfly.top/gtovnrcyht.html

C#:   public override string ToString() => Name;
来源：http://hz.shangyingyoupin.top/gtvmfmeggj.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gteupllgry.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtwfzddxyb.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtsqrrenqa.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtfxtvvlqi.html

TS:   u instanceof User
来源：http://hz.jinqigufen.top/gtlfrlbdep.html

Java: u instanceof User
来源：http://hz.pengpengdd.cyou/gturrntykl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhaomingkeji.xyz/gticrodkzv.html

Ruby: u.is_a?(User)
来源：http://hz.jqgfzy.top/gtjpfdjftn.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtjvbakave.html


<!-- 参考信息 -->