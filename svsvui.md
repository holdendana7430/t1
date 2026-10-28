代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangdashe.top/gtfflmffmv.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtolbiktkw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydzc1.top/gtyqnpxfvs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.0kj1m.cn/gtuokjbufm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aizwys.cn/gtbynehoqe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jlsjyb.cn/gtpulxwudm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shangyingyoupin.top/gtkmlofhvk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hysaishi.cn/gtlliuedzw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gtfwicdcbd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangdashe.top/gtxjiofasb.html

[E16] 数字千分位
来源：http://hz.chenjidiqi.icu/gtrmyhrykc.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gttpeilbqa.html

PHP:  number_format(1234567);
来源：http://hz.andypj.xyz/gtiyyuckrd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gtjbdcqyxj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtmmdxmgny.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgfzy.top/gtxjhohegu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtxedmhlno.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinghuilouyu.cn/gtnxepkzyi.html

C#:   1234567.ToString("N0")
来源：http://hz.chenlongwang.top/gtwznhsrjt.html

[E17] 首字母大写
来源：http://hz.dianchejie.cn/gttbixmccr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtqhkolseg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtcvszuctw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gttbralawv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtjsizwkcs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtvlyjjomf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtvpvpfgug.html

Ruby: s.capitalize
来源：http://hz.shzxlz.cn/gtymcepzke.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtlqjfuajp.html

[E18] 模板占位符替换
来源：http://hz.zhiwuduotai.top/gtjsqhdjal.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangdashe.top/gtdzggljvz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.quarkkingdee.top/gtkfzdzfmy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtiavpohfx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtpnlgdglt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtdqsjwumb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhoulong.xyz/gtifwbqkcx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fzhhl.top/gtzvhxtbco.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtginrsbqh.html

[E19] 多行文本按行拆分
来源：http://hz.tanke756.top/gtzrvbflnz.html

Py:   s.splitlines()
来源：http://hz.zycfv.cn/gtoxvdrmgy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuanzx.com/gtfhybxsti.html

JS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtsgwuedlp.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtpgcybhgk.html

Java: s.lines().toList()
来源：http://hz.0kj1m.cn/gtqlevzrfn.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gthvlilubw.html

Ruby: s.lines
来源：http://hz.xingfuxueyuan.xyz/gtjutzfvth.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gttqwjzljq.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gtxynyxxnl.html

Py:   if not s:
来源：http://hz.wangdashe.top/gtxkmskygo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dianchejie.cn/gtkduuhlop.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gtkzohqiwu.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtqsumoasx.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtkdbgiwve.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangkeji.top/gtcpvkuiyd.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtoastucvk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtvbetrtrt.html

[E21] 超长截断加省略号
来源：http://hz.sufxvd.cn/gtjpxaiqpi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.316326.xyz/gtayqsohdr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtdflwbwlj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtrdkgrsnc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gttnhfnkmt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtighilfrj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhaomingkeji.xyz/gtyxhknutt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtgywaofpx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtlvkrzyyt.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gtdtpkweub.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daria6918.cn/gtlcszhfdz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtjngmtfel.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtdsbtfhyl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtgrcemzxk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhixingplan.top/gtyshlfqew.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.havefunace.top/gtwozojnmb.html

Ruby: s.bytesize;  s.length
来源：http://hz.c1oappe.top/gttyopyxka.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtdteddyaf.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqmgiabbb.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtygragfra.html

================================================================================
来源：http://hz.cdnleiting.top/gtgsqisssi.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtzkfzothv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gttphzzenb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtuwulcekp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenlongwang.top/gtipihltau.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dianchejie.cn/gtltyxckjf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtavdcxkin.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.52xcode.cn/gtbexvosou.html

Ruby: File.read("a.txt")
来源：http://hz.feifeiyinyue.top/gtcjjupdzt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.smart0.xyz/gtmqgpmpdl.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gtxltnohdx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.316326.xyz/gtiknicodc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtwzzsvpzk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gttuehxzvy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtvgizyrru.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtemhbsxlp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydjk.org.cn/gtemlveazi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.svipenyu.cn/gtadwmmfox.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.meibo888.top/gttzuoabpp.html

[F03] 写入文件（覆盖）
来源：http://hz.hammf.cn/gtfqghhmlf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ppjwa.cn/gtanaexjww.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtjkfxycva.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtzglciqzk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtzeencoxz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtqorygood.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtuzqhdrme.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtneulvnzv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuxming.cn/gtqrwhscli.html

[F04] 追加写入文件
来源：http://hz.hysaishi.cn/gteyveqcqq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xinyue.icu/gtjxqpcumn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.quarkkingdee.top/gtgsoxusyq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtnjpqfbaw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtzttegvsm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yangfankeji.com/gtnbkndcwb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cheryme.top/gtehfpnhbn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jlsjyb.cn/gtqjdbnmeu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xylfe.cn/gtyzqqpsra.html

[F05] 判断文件或目录是否存在
来源：http://hz.quarkkingdee.top/gthpuwgegx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhijiandao.cn/gtdexpomne.html

PHP:  file_exists("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtdqpnxerq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtjvnksatx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtwwvhwdlq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtlkzqlmiu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sweek.top/gtgwqkljfd.html

Ruby: File.exist?("a.txt")
来源：http://hz.sxryk.cn/gtfxafunih.html

C#:   File.Exists("a.txt")
来源：http://hz.zhixingplan.top/gtauyhlrlj.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtcqmiwvaw.html

Py:   os.remove("a.txt")
来源：http://hz.yueranfly.top/gtgvwczlkr.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gtvxdemsqo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtjywmzzke.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gteymumirx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtziaalmcu.html

Go:   os.Remove("a.txt")
来源：http://hz.daxiang520.top/gtwodjdgwq.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gthbqpdbyx.html

C#:   File.Delete("a.txt");
来源：http://hz.snrcjt.cn/gtyfpvbrqq.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtxciwzama.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtueriizaz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtbuovrrxw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtxzpbekpc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtbgsveydx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tian-w.cn/gtudxzgirl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ppjwa.cn/gtjoyoswlv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sweek.top/gtpkumfcuj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtvpoghowk.html

[F08] 遍历目录
来源：http://hz.wangdashe.top/gtcoefgcgq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gthykncohs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gogol.net.cn/gtcruierhn.html

JS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtgwodirbj.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtuecpzjae.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtndumfjag.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sysykeji.top/gtkppbfcaj.html

Ruby: Dir.children("dir")
来源：http://hz.xylfe.cn/gtfhiggqub.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtujjwlhhf.html

[F09] 获取文件大小
来源：http://hz.chenjidiqi.icu/gtmvbndhud.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuxming.cn/gtwpuzmclb.html

PHP:  filesize("a.txt");
来源：http://hz.vqdsnc.cn/gtmdxqhcbl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtmpmjaqvz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtdurbcsmf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gttmyuhnpj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.bjfxy.top/gtbeaujeko.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtcfiybako.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.svipenyu.cn/gtphaayhez.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtgovfiaxu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtazrbofjk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gtycbiwmvz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtyuuwczlq.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtbzivsbjl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yanxiufei.cn/gtafmyuaag.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtmimwhpkb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtmhhjophk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aibaodan.cn/gtvkmnzsew.html

[F11] 复制与移动文件
来源：http://hz.ybcxt.top/gtilvoyjun.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtswqtelub.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gotoacloud.top/gthnyoelbz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gttvreucve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtfftwnlzf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtsyhaoevi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtwxrhtcgc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtoionzpcx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gotoacloud.top/gtkxkhagtu.html

[F12] CSV 读写
来源：http://hz.snrcjt.cn/gtebtlkbri.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gtatdmspdr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhengqikj.top/gtezupoeea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtateprgft.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtpfccgzlc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.0kj1m.cn/gtmoqzqlxi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtujiajlua.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtctdzqmux.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtvbrtyoav.html

================================================================================
来源：http://hz.9152youxi.cn/gttdcegvnx.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtlzotbixh.html

================================================================================
来源：http://hz.zhijiandao.cn/gtfqjdydbb.html

[G01] 定义类
来源：http://hz.pengpengdd.cyou/gtekoepfrg.html

Py:   class User: pass
来源：http://hz.fzhhl.top/gtbfmdegmp.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtwgzhlmsg.html

JS:   class User {}
来源：http://hz.shanyushiyangtech.top/gtxchyhozd.html

TS:   class User { name: string = ""; }
来源：http://hz.9152youxi.cn/gtxucgnghk.html

Java: class User {}
来源：http://hz.nanxuanxn.top/gtnpmqmvtj.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtahqjeaas.html

Ruby: class User; end
来源：http://hz.ydjk.org.cn/gtcodhstqg.html

C#:   class User {}
来源：http://hz.shangyingyoupin.top/gtjvlzozbp.html

[G02] 构造函数
来源：http://hz.c1oappe.top/gtqhjuisaj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydzc1.top/gtwdwytscr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.smart0.xyz/gtqkpargcb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gtkkrnvtsq.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gtqpbjdcxz.html

Java: User(String name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtoqugoraz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuxming.cn/gtvusqaxoo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fzhhl.top/gtypsottbz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gtxlpqxirg.html

[G03] 实例属性
来源：http://hz.quarkkingdee.top/gtdxnpyldg.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtuuyucjdc.html

PHP:  public string $name = "x";
来源：http://hz.sysykeji.top/gtlkzkfpkd.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtxdnidgls.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtrpywstii.html

Java: private String name;
来源：http://hz.cashguo.top/gtjkzmisxg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtlbbefmqx.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtlswiugaq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtvezhngnb.html

[G04] 定义方法
来源：http://hz.316326.xyz/gthuclzrcu.html

Py:   def greet(self): return self.name
来源：http://hz.haohaochexian.top/gtagmomknr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtjofguuit.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258888.top/gtsqbxwuuy.html

TS:   greet(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtngcldqro.html

Java: String greet() { return name; }
来源：http://hz.9152youxi.cn/gtghazakta.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtmhgdqobn.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtrxhngfcy.html

C#:   public string Greet() => Name;
来源：http://hz.feifeiyinyue.top/gtgjiorrge.html

[G05] 继承
来源：http://hz.andypj.xyz/gtuyoufncc.html

Py:   class Admin(User): pass
来源：http://hz.yuanzhike.top/gtgrutebmg.html

PHP:  class Admin extends User {}
来源：http://hz.mhx1999.top/gtitbqilyo.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtwzenhqcc.html

TS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtyurzyket.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtxhebixfx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.316326.xyz/gtypnqfdug.html

Ruby: class Admin < User; end
来源：http://hz.jinqigufen.top/gtkkptosek.html

C#:   class Admin : User {}
来源：http://hz.guowangkeji.top/gtuidfkzsi.html

[G06] 重写方法
来源：http://hz.cdnleiting.top/gtoiiitgfi.html

Py:   def greet(self): return "admin"
来源：http://hz.bjfxy.top/gtyzdhvsry.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtpwisojtq.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtlxczyhbx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtorxdkgqg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gttitwfyrw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtjvpmpuoo.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtaepkeyfr.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangdashe.top/gtalkgpfpj.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtjdhhypjd.html

Py:   super().greet()
来源：http://hz.sweek.top/gtycpkijox.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gttkyuswmc.html

JS:   super.greet();
来源：http://hz.shuidangran.top/gtsrioriyr.html

TS:   super.greet();
来源：http://hz.yanxiufei.cn/gtmhnidecq.html

Java: super.greet();
来源：http://hz.yuxming.cn/gtqnukrazm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aizwys.cn/gtpbwqdbik.html

Ruby: super
来源：http://hz.xuanzx.com/gtyjehvtsv.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtisaspoaz.html

[G08] 静态方法与属性
来源：http://hz.feifeiyinyue.top/gtuxnqepvi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.quarkkingdee.top/gtdrzgqajq.html

PHP:  public static function f() {}
来源：http://hz.gogol.net.cn/gtvzgmvgln.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gttgcjhibw.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gthsljooha.html

Java: static void f() {}
来源：http://hz.andypj.xyz/gtixhogddj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtzeatavfy.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtudufrlkj.html

C#:   public static void F() {}
来源：http://hz.sufxvd.cn/gtxagjcvzd.html

[G09] 接口 / 抽象类
来源：http://hz.xziqi.cn/gtklaqreif.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cdnleiting.top/gthdeodpyo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtcwbvibny.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuanzhike.top/gtnixnfnqi.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydzc1.top/gtkjkicecc.html

Java: interface Shape { double area(); }
来源：http://hz.hysaishi.cn/gtmgsphcmz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtajajekct.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.andypj.xyz/gtalqklojg.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gteifauwuu.html

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtdgnqegfh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtiwuifjzg.html

PHP:  public / protected / private
来源：http://hz.birdmap.top/gtactkwynx.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtswdtouul.html

TS:   public / protected / private
来源：http://hz.jqgfzy.top/gtxeqeslby.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gtnmvlprjg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigufen.top/gterntensd.html

Ruby: public / protected / private
来源：http://hz.cheryme.top/gtqqvnfcdo.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtldhwvyhh.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtktvnkfew.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtifzzalat.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtxaflptdt.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtiqtdmczh.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtsyftniia.html

Java: public String getName() { return name; }
来源：http://hz.ivvv.top/gtybimuwhj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtptnqpjpa.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtbhrigtrd.html

C#:   public string Name { get; set; }
来源：http://hz.chenjidiqi.icu/gtgtmpigqy.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtwhvsmity.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtbvupnyhc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtblyemant.html

JS:   toString() { return this.name; }
来源：http://hz.jlsjyb.cn/gtfbsqkegt.html

TS:   toString(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtnungjvkp.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gthuktzqxj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gtciouyzvg.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gtnlqxqcmv.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtrrcnzplu.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtpzpaqecy.html

Py:   isinstance(u, User)
来源：http://hz.sufxvd.cn/gtwgbanuol.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtwjhbkqct.html

JS:   u instanceof User
来源：http://hz.hywenlv.cn/gtydbczuau.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtsrfdvxgf.html


<!-- 参考信息 -->