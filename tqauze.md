代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.0kj1m.cn/gtcdbyqzjb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.quarkkingdee.top/gtapsuvcel.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gthkqbxyhn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtldqkoobo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtbmifrhok.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtrzqxsrty.html

[E16] 数字千分位
来源：http://hz.tianlin.xyz/gtduqsczrh.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gtosokwlqa.html

PHP:  number_format(1234567);
来源：http://hz.birdmap.top/gthouuptnh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gteeigagoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gteoifwmyu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.kuanghao11.cn/gttrusbkja.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.quarkkingdee.top/gtmaqnamue.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhixingplan.top/gthnogadth.html

C#:   1234567.ToString("N0")
来源：http://hz.zhoulong.xyz/gtubpwjywy.html

[E17] 首字母大写
来源：http://hz.wangshuangyany.cn/gtrrcyasws.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangdashe.top/gtecxinugf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gthryfhyxi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtfkqnduvw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtzhmhodnx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhaomingkeji.xyz/gtroecoltu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtylkzghmk.html

Ruby: s.capitalize
来源：http://hz.zhijiandao.cn/gtbcuxyjqy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258888.top/gtyyursyct.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gteofnnmic.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gthsxesurw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuxming.cn/gtkcbqlgxg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtwmavqqib.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtnhfazism.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dashuyun.cn/gtxkenljoe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258.top/gtvxwusbks.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtdghkvoro.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dianchejie.cn/gtlhtxkmij.html

[E19] 多行文本按行拆分
来源：http://hz.gotoacloud.top/gtrlxitmst.html

Py:   s.splitlines()
来源：http://hz.yanxiufei.cn/gtfxzcsayl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtgwqvksqt.html

JS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtpvhxnjuk.html

TS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtsbmnnspx.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gttlhyvbft.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhongyouzk.top/gtoiwlvotx.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtesfhscfh.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtceedkjss.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtydohwcwv.html

Py:   if not s:
来源：http://hz.hongshengwenyu.top/gtuisxdeqm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtjcpfqfki.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenlongwang.top/gtdxryazsc.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gtizejohqy.html

Java: if (s.isEmpty()) {}
来源：http://hz.tanke756.top/gtapiepzet.html

Go:   if s == "" {}
来源：http://hz.yj20258.top/gtgybsqkla.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtryhhaatg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtycdtpgad.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtivufevfl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gtazzsnmfp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dianchejie.cn/gtjqxkrsgq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtfmygwjmk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtcajzyyok.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtrhtggilo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenjidiqi.icu/gthvpohqju.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gogol.net.cn/gtefyqussj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yongpay.top/gtenyxnzuj.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtaspdulzf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtxcepavlb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gthjdpkevx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtdescipqd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtnwgjomeq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.316326.xyz/gtubsarmsj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ybcxt.top/gtuvfythyj.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtuquwtviu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.redwolf501.top/gtlsavnvxg.html

================================================================================
来源：http://hz.zdqjudy.top/gtpgydzrzj.html

F. 文件与目录
来源：http://hz.cashguo.top/gtbxximsvg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcclenyxl.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtskxynehx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtctjibpko.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenlongwang.top/gtycolerpd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtoaibmgtm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jlsjyb.cn/gtdaxuxxdb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtchjybctn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yongpay.top/gthvvpwxvu.html

Ruby: File.read("a.txt")
来源：http://hz.snrcjt.cn/gticrfkrvw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ivvv.top/gtwowzyhro.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gttbdsiizj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.vqdsnc.cn/gtkqkqches.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.daria6918.cn/gtxlggopxt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtljjhliec.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtbvpwipfd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtgphcgxwk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gtzvakrtqx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtenxixtod.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj202588.top/gtrxfjpnsn.html

[F03] 写入文件（覆盖）
来源：http://hz.mhx1999.top/gtmfnbzguv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenlongwang.top/gtyamyzled.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtmkelxhcs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gttfkgyaxw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gtztdfkbak.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhaomingkeji.xyz/gttjuzpbak.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shzxlz.cn/gtntboeyht.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guowangkeji.top/gtzpukruui.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtpzcydlgm.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gtkhjqfdyd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xziqi.cn/gtxskdgvap.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jyoumei.cn/gtictwuwoq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtcfrolszu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtylwphwqb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhixingplan.top/gtiwrdwkwi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtuyyinijp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtsprlawro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gttmgvlakb.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gttfbrytan.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nwbrower.top/gtnkynrrun.html

PHP:  file_exists("a.txt");
来源：http://hz.ppjwa.cn/gteguukark.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtmzvabyry.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtkzdctjzd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtecrkdupc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aibaodan.cn/gtiyqgmgvn.html

Ruby: File.exist?("a.txt")
来源：http://hz.jlsjyb.cn/gtebpyeubk.html

C#:   File.Exists("a.txt")
来源：http://hz.52xcode.cn/gtmhxzrlvc.html

[F06] 删除文件
来源：http://hz.xuetiantiany.cn/gtpoorirrd.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtgvjkwyqx.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gtghmnuypp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtutmfomjc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtploikapn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtvsfzvtcu.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtnifuetgb.html

Ruby: File.delete("a.txt")
来源：http://hz.zycfv.cn/gtbqjsvsaf.html

C#:   File.Delete("a.txt");
来源：http://hz.cdnleiting.top/gtbuzufden.html

[F07] 创建目录（含多级）
来源：http://hz.xziqi.cn/gtwzfhccpw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtybjvwtwc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtqwnzbryr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtahptwnkv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtgkhimbof.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shzxlz.cn/gtcbtjhato.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtyrqwkaew.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daria6918.cn/gthwqmcwjn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gtymknfstw.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gthjcvdrnl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gteeyitwru.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gtyzmscyew.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtutepgzkp.html

TS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtgeqqknml.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtyvsaijlh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gtrsxbqite.html

Ruby: Dir.children("dir")
来源：http://hz.zhiwuduotai.top/gtsiggjjhi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhiwuduotai.top/gtvwktdbsq.html

[F09] 获取文件大小
来源：http://hz.0kj1m.cn/gtlcizhkkf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigufen.top/gteecosjpx.html

PHP:  filesize("a.txt");
来源：http://hz.fengsongda.top/gtyexwiuvy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtvxtvrwzz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtfpbmkodf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtknrsmpad.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangshuangyany.cn/gtmpiotpnk.html

Ruby: File.size("a.txt")
来源：http://hz.cqqwz.cn/gtesoymmaf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xinyue.icu/gtajqheymz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shangyingyoupin.top/gtfeiyxfxc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtigvjakpf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.52xcode.cn/gtcduukybe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtawbphedk.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtgjzdrgee.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydjk.org.cn/gtmxtpwnfn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtxchufhcl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtujgbkaek.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtjgpadcub.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtihdsqucc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtqdbfzkwd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtmpwsdwao.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtuvucmqrq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtjgxgxpji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gtrlbtfrim.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.0kj1m.cn/gtdmjnhojp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtjjnjlbri.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtgfohhavu.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gtcncowvcw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtjilzjfdz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ybcxt.top/gtjubmeobz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gogol.net.cn/gtmepwuohw.html

TS:   // 同上
来源：http://hz.xuanzx.com/gtbtavixcw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtpdkytoke.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.52xcode.cn/gtrvkhwwzn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuanzhike.top/gtjockdoio.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gtgehhaptf.html

================================================================================
来源：http://hz.fengsongda.top/gtgvjunlkv.html

G. 面向对象
来源：http://hz.smart0.xyz/gtttsjxisv.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtelkbpang.html

[G01] 定义类
来源：http://hz.jinqigfzy.top/gtishlhnnd.html

Py:   class User: pass
来源：http://hz.zdqjudy.top/gtiaabcqcq.html

PHP:  class User {}
来源：http://hz.ehwqpu.com/gtughjqobd.html

JS:   class User {}
来源：http://hz.vqdsnc.cn/gtuhbsxjwc.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtbtcpdvho.html

Java: class User {}
来源：http://hz.wangdashe.top/gtjazplsni.html

Go:   type User struct { Name string }
来源：http://hz.jinghuilouyu.cn/gtinenpqwm.html

Ruby: class User; end
来源：http://hz.yuxming.cn/gttgrisemo.html

C#:   class User {}
来源：http://hz.kuanghao11.cn/gtaosnppic.html

[G02] 构造函数
来源：http://hz.shanyushiyangtech.top/gtimzncath.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhaomingkeji.xyz/gtbfegnwtb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgfzy.top/gtnrjrveeb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtqgniapip.html

TS:   constructor(public name: string) {}
来源：http://hz.jyoumei.cn/gttjeeruyz.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtwyristsc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtjfdmsjci.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.vqdsnc.cn/gtildrinap.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tanke756.top/gtzguibjss.html

[G03] 实例属性
来源：http://hz.jyoumei.cn/gtmsisishh.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtucwsdhde.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gttexpcbjh.html

JS:   this.name = "x";
来源：http://hz.xuanzx.com/gtdoyayekf.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtybudgwwx.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtugwifwlb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gthkrwxvhm.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtyijzmkbr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gogol.net.cn/gtfgahxydi.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtxafigxzx.html

Py:   def greet(self): return self.name
来源：http://hz.iojbl.cn/gtargivnfi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtidbvtfmb.html

JS:   greet() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtlezmfsrh.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtidyjwdud.html

Java: String greet() { return name; }
来源：http://hz.nanxinkj.top/gtcwnsfush.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gtwpnszllt.html

Ruby: def greet; @name; end
来源：http://hz.jianghu66.top/gtczllfiww.html

C#:   public string Greet() => Name;
来源：http://hz.zhaomingkeji.xyz/gttzzestyu.html

[G05] 继承
来源：http://hz.guannengcc.top/gtrevrgfbk.html

Py:   class Admin(User): pass
来源：http://hz.feifeiyinyue.top/gtydyurikz.html

PHP:  class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtuhiytqrh.html

JS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtcpimxsgk.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtkpoonfyj.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtohxcbowa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tianlin.xyz/gtqvfvzgiz.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtvancghgm.html

C#:   class Admin : User {}
来源：http://hz.hnxiangtu.top/gtpzrubxnt.html

[G06] 重写方法
来源：http://hz.daria6918.cn/gtwuiyngff.html

Py:   def greet(self): return "admin"
来源：http://hz.sxryk.cn/gtzrqlezel.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtpmgbxcha.html

JS:   greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtldgeebtz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtvigjgzli.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yonumen.top/gtdkmidthw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hywenlv.cn/gtlfhbxhsq.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtmjqzbluu.html

C#:   public override string Greet() => "admin";
来源：http://hz.vqdsnc.cn/gttrcqhldj.html

[G07] 调用父类方法
来源：http://hz.tianlin.xyz/gttycdfnay.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtadzfdtxc.html

PHP:  parent::greet();
来源：http://hz.0kj1m.cn/gtnahnntft.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gthbwsvkff.html

TS:   super.greet();
来源：http://hz.zycfv.cn/gtjjdmiqjn.html

Java: super.greet();
来源：http://hz.jyoumei.cn/gtljxnmluj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gogol.net.cn/gttzzqtrhj.html

Ruby: super
来源：http://hz.jinghuilouyu.cn/gtjstukiij.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtodvmdznh.html

[G08] 静态方法与属性
来源：http://hz.wangshuangyany.cn/gtddmhuxgw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtwaegawfh.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtknbzyzxf.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtfmujepnn.html

TS:   static f(): void {}
来源：http://hz.jiagoushi.top/gtunpakagi.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gtznfhdoer.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtegwrifrk.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gtkpfpztsd.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtdjyzrrwo.html

[G09] 接口 / 抽象类
来源：http://hz.ydzc1.top/gtjcqoeuel.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtrcqkmmzt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258888.top/gtlvshuptg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtgicessiv.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtceetjnbv.html

Java: interface Shape { double area(); }
来源：http://hz.316326.xyz/gtytekrwvy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtvvdnnicl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhengqikj.top/gtbrvixqew.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtekicvydf.html

[G10] 访问控制
来源：http://hz.quarkkingdee.top/gtibilatvm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtqbwgkput.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtmwsjodze.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258.top/gtdnrawjas.html

TS:   public / protected / private
来源：http://hz.bjfxy.top/gtepanipjs.html

Java: public / protected / private / 默认包级
来源：http://hz.aibaodan.cn/gtmjjulwsq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tianlin.xyz/gtllcfsbmb.html

Ruby: public / protected / private
来源：http://hz.ydjk.org.cn/gtumcnwryt.html

C#:   public / protected / private / internal
来源：http://hz.zdqjudy.top/gtzucvwyet.html

[G11] getter / setter
来源：http://hz.tianlin.xyz/gtrlekducg.html

Py:   @property 与 @x.setter
来源：http://hz.sufxvd.cn/gtaukfzvyl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtwslkrqwn.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtvgexfdnq.html

TS:   get name(): string { return this._name; }
来源：http://hz.ivvv.top/gtjvjphlmt.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gtgyuzuvuy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtmnmeabhc.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gtyfmdgpmg.html

C#:   public string Name { get; set; }
来源：http://hz.snrcjt.cn/gtdwocuwjg.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtwkfudcil.html

Py:   def __str__(self): return self.name
来源：http://hz.yj202588.top/gttfpqqlnw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtmlfjupzq.html

JS:   toString() { return this.name; }
来源：http://hz.yueranfly.top/gtzpazfvms.html

TS:   toString(): string { return this.name; }
来源：http://hz.yuxming.cn/gtrkgixziq.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gteiwzhprz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yvedp.cn/gtshmtitua.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtkehpitbu.html

C#:   public override string ToString() => Name;
来源：http://hz.jlsjyb.cn/gtbnpxwjsk.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gtkbyntwjg.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtprvmctjl.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gtfrmbokyc.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtamlxolvl.html

TS:   u instanceof User
来源：http://hz.yuanzhike.top/gtlfqzcypz.html

Java: u instanceof User
来源：http://hz.hfpthk.cn/gtuudoghjp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtyvqoxofj.html

Ruby: u.is_a?(User)
来源：http://hz.meibo888.top/gtaeevyikw.html

C#:   u is User
来源：http://hz.svipenyu.cn/gtgwqkujhx.html


<!-- 参考信息 -->