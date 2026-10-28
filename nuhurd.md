代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gaohongyu789.top/gtidysltng.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhaomingkeji.xyz/gtvxezirzu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhaomingkeji.xyz/gtitqrmlno.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtibrnqcqz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.c1oappe.top/gtaoxjuhox.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtbocdfktt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtucoxlqct.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhengqikj.top/gtfqnifxby.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gttcuuules.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangtech.top/gtpriautvk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtwulggnud.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gteymvzxtx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hammf.cn/gtvzetfuim.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtahedaibj.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtvfbznppw.html

Py:   f"{1234567:,}"
来源：http://hz.cqqwz.cn/gtqlobdjvp.html

PHP:  number_format(1234567);
来源：http://hz.52xcode.cn/gtrzefclmz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtdiwjqodj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtmtcpuucb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tian-w.cn/gthcjaemyy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dashuyun.cn/gthsqzkpbd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtzfhbjdnl.html

C#:   1234567.ToString("N0")
来源：http://hz.snrcjt.cn/gtiixcbhwq.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gtelkwksgo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.havefunace.top/gtwwwdtzqp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sysykeji.top/gtuigddsbd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtftbwcwcd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtpdpjyqjo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cashguo.top/gttvflzqwi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.mhx1999.top/gtnnhjmnhq.html

Ruby: s.capitalize
来源：http://hz.aizwys.cn/gtueuxfbpf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gttotmwuoe.html

[E18] 模板占位符替换
来源：http://hz.ehwqpu.com/gtdoekxzeu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtbftukoij.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtaubwnpce.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtuiaepkyx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtfarzvkkh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtzuifkmqx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fzhhl.top/gtqzrnppjt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jianghu66.top/gtobnmflis.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtapjgxcph.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtarfoafsu.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gttqdcdaia.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jyoumei.cn/gtyplbxfin.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtehyogiuj.html

TS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtskbkweza.html

Java: s.lines().toList()
来源：http://hz.mhx1999.top/gtxbpcrjdz.html

Go:   strings.Split(s, "\n")
来源：http://hz.daxiang520.top/gtraczpabc.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtxoouibfj.html

C#:   s.Split('\n')
来源：http://hz.pycfn.com/gtrqxeaies.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtwuummahv.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtqodoeysk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ybcxt.top/gtbqsldkxs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jiagoushi.top/gttozcvqxj.html

TS:   if (s === "") {}
来源：http://hz.yj20258888.top/gtjxmflyyz.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gtvywbcxsq.html

Go:   if s == "" {}
来源：http://hz.tianlin.xyz/gtxnalqlaj.html

Ruby: if s.empty?
来源：http://hz.yuxming.cn/gtkxvjtyfz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gogol.net.cn/gtvxulliot.html

[E21] 超长截断加省略号
来源：http://hz.gotoacloud.top/gtddachxsw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aizwys.cn/gtlwkfdnhd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sysykeji.top/gtaxwezdtt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtjttgybum.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtyhemynel.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtrvxrcrij.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtourdtgnk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yueranfly.top/gtcawsvyeh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.bjfxy.top/gtmofjqdol.html

[E22] 字节长度与字符长度
来源：http://hz.aizwys.cn/gtpelcdeyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gtxhdmympx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtcpyirkjg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtikgjecza.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtcmquirvr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yvedp.cn/gtrdeitopq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shzxlz.cn/gtjafhpznu.html

Ruby: s.bytesize;  s.length
来源：http://hz.tanke756.top/gtvsxurvcu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aibaodan.cn/gtjqaowsae.html

================================================================================
来源：http://hz.yongpay.top/gtzhuxhoof.html

F. 文件与目录
来源：http://hz.nwbrower.top/gttkjbjycd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtrvzcvauh.html

[F01] 读取整个文件
来源：http://hz.daxiang520.top/gtytnrcfbt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jlsjyb.cn/gtjpezofpk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.andypj.xyz/gtstiwqhzw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtfauncirx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtcpkvbypa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtsewglcid.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtoyeckokc.html

Ruby: File.read("a.txt")
来源：http://hz.chenlongwang.top/gtwszbursg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.bjfxy.top/gtyfetfuqp.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtgyoyiyno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangshuangyany.cn/gteiivhgfa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtmxrtvava.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtwdfdxcqx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtulqdscoj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gthibpvdue.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gtqnvkdgmb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.vqdsnc.cn/gtngcjjmvw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtrhrxiknk.html

[F03] 写入文件（覆盖）
来源：http://hz.ydjk.org.cn/gtmedwqbbm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtggtbyxdj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtcqhwtnex.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtnktwfebu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtrbyamsah.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtyozgigyy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtytpkdqdo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.vqdsnc.cn/gtupqlxvbh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yueranfly.top/gtlplplies.html

[F04] 追加写入文件
来源：http://hz.c1oappe.top/gtwbovdsjr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtcokjinbv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guannengcc.top/gtxixzpdlj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtosddojaf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gtoczsmerp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jyoumei.cn/gtgldnzzar.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtwzlryrrm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtlfqpnzda.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cdnleiting.top/gtkozbejag.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtoilozawa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xingfuxueyuan.xyz/gttbxsjcks.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtsmhhdcgn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gttfpvdroi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtkhxxmpzc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtjeelaous.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gtsorobfpp.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigfzy.top/gtsbvhkogo.html

C#:   File.Exists("a.txt")
来源：http://hz.dianchejie.cn/gtbywuqlpp.html

[F06] 删除文件
来源：http://hz.wangshuangyany.cn/gttgfnsdmt.html

Py:   os.remove("a.txt")
来源：http://hz.dashuyun.cn/gtepkmdjbe.html

PHP:  unlink("a.txt");
来源：http://hz.cucudq.cn/gtwtalppuu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtwdwdpbub.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtapggfpoe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtayubouqg.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtlnxiifns.html

Ruby: File.delete("a.txt")
来源：http://hz.meibo888.top/gthsqqfnbv.html

C#:   File.Delete("a.txt");
来源：http://hz.nwbrower.top/gtjyvzaopb.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtfjiiasho.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangkeji.top/gtschduyrq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sweek.top/gtlrpmbtwp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtvqbiaiul.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtjfocpzms.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.bjfxy.top/gtawcfzhnz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtynyvtczi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yonumen.top/gtrnejnsew.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ehwqpu.com/gtmfwninpc.html

[F08] 遍历目录
来源：http://hz.hammf.cn/gtmwemlemy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gtgfeefcbk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtgnjdxhmh.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtxmtqzkft.html

TS:   fs.readdirSync("dir")
来源：http://hz.daxiang520.top/gtuembpygj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtknvjgeuk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.c1oappe.top/gtflrlresd.html

Ruby: Dir.children("dir")
来源：http://hz.birdmap.top/gtzwdfmuqr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shuidangran.top/gtohnppfpl.html

[F09] 获取文件大小
来源：http://hz.cheryme.top/gtcwuetqaw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gtxjlofuyp.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtbsygfphw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtdjhkurti.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtqlfbieio.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtbmsmcdto.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtdryyvimg.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtzkfcydfb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtonzhxfqf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtwcvscbpw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtlduzxipa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hysaishi.cn/gtglaohvrk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtvtxpqegr.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gtirihglgb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gtxogxwuma.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtukhymods.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gthyqerzcl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtowlnesek.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtudyyiwek.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtolcgtlvh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ybcxt.top/gtexgzkgje.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtelkzouuc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtywsskknk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sweek.top/gtuyfticnj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtggzhkeon.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtpgbzhyhu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtqcbmeadv.html

[F12] CSV 读写
来源：http://hz.ywan-chungtsiang.top/gtcxhdukeq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yvedp.cn/gtnnxzsxqj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.meibo888.top/gtuxvimibw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.9152youxi.cn/gtoazmztal.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtqmppwrmy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtzdxxqbyo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aibaodan.cn/gtgvvahiky.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtxfvigvbe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangkeji.top/gtyfptbyau.html

================================================================================
来源：http://hz.andypj.xyz/gtnmvlxjhx.html

G. 面向对象
来源：http://hz.meibo888.top/gthocvqwqg.html

================================================================================
来源：http://hz.aibaodan.cn/gthcurdomb.html

[G01] 定义类
来源：http://hz.cqqwz.cn/gtgyxzbvlq.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gtnlausgps.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtvoblbzka.html

JS:   class User {}
来源：http://hz.pengpengdd.cyou/gthichoahk.html

TS:   class User { name: string = ""; }
来源：http://hz.tianlin.xyz/gtjhrqyjbu.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtywtsgnvc.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gtudrtidli.html

Ruby: class User; end
来源：http://hz.daxiang520.top/gtzpwijkiw.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtvvxskshx.html

[G02] 构造函数
来源：http://hz.ivvv.top/gtxipdbfbx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtvuhdoiiq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtbmzzthvz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtyupmiezu.html

TS:   constructor(public name: string) {}
来源：http://hz.xinyue.icu/gtdkzlcgkt.html

Java: User(String name) { this.name = name; }
来源：http://hz.fengsongda.top/gtovyigfgq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.andypj.xyz/gtbjorgkqa.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangdashe.top/gtsgfuagdh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gthfiogdpg.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtizeyjfsf.html

Py:   self.name = "x"
来源：http://hz.jlsjyb.cn/gtxiswqohe.html

PHP:  public string $name = "x";
来源：http://hz.chenzaomai.com/gtqksynslm.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtphaqfquw.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gticwjjghp.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtsnondxkd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtxjjzznuq.html

Ruby: @name = "x"
来源：http://hz.yongpay.top/gtcnnksazy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtwoqxtpts.html

[G04] 定义方法
来源：http://hz.guowangkeji.top/gthxczoysi.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtdhqptxxu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtyqnxfvry.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gttjgrwiha.html

TS:   greet(): string { return this.name; }
来源：http://hz.meibo888.top/gtfeaevnyg.html

Java: String greet() { return name; }
来源：http://hz.sysykeji.top/gtfuigtzwo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuxming.cn/gtkbqskquk.html

Ruby: def greet; @name; end
来源：http://hz.bjfxy.top/gtcxzfumvt.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtazpadosm.html

[G05] 继承
来源：http://hz.yueranfly.top/gtornwsulg.html

Py:   class Admin(User): pass
来源：http://hz.aibaodan.cn/gtmayajhhz.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtmhxtgkzj.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gttkpvipzq.html

TS:   class Admin extends User {}
来源：http://hz.cashguo.top/gttdqxkywx.html

Java: class Admin extends User {}
来源：http://hz.0kj1m.cn/gthxguolut.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtlnpfjutm.html

Ruby: class Admin < User; end
来源：http://hz.jinyuanbaomall.cn/gtbuigllrf.html

C#:   class Admin : User {}
来源：http://hz.yj20258888.top/gtjrtmepkl.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtupjaftpq.html

Py:   def greet(self): return "admin"
来源：http://hz.zhixingplan.top/gtvwdeamka.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtscjivnuw.html

JS:   greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtfudqtuqe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtniulpszw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtofwnfiwh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtzltcmzpj.html

Ruby: def greet; "admin"; end
来源：http://hz.sufxvd.cn/gtyqxbtcfq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtiosggwoz.html

[G07] 调用父类方法
来源：http://hz.mhx1999.top/gtodjmofrh.html

Py:   super().greet()
来源：http://hz.redwolf501.top/gtejrfcrbv.html

PHP:  parent::greet();
来源：http://hz.feifeiyinyue.top/gtaeqewlpv.html

JS:   super.greet();
来源：http://hz.yj20258888.top/gtxitpysme.html

TS:   super.greet();
来源：http://hz.vqdsnc.cn/gtxxnqwoid.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gtuttueeie.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nwbrower.top/gtwxxfwpuu.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtxkzkbcjk.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtcutivdwa.html

[G08] 静态方法与属性
来源：http://hz.yvedp.cn/gtrtirtwwa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgfzy.top/gtymrogypa.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtmlonwzav.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtdxitxniz.html

TS:   static f(): void {}
来源：http://hz.cucudq.cn/gtdgjdvyoa.html

Java: static void f() {}
来源：http://hz.smart0.xyz/gtymewoszu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtyhkvzdqr.html

Ruby: def self.f; end
来源：http://hz.haohaochexian.top/gtjshoszca.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtravbjzsk.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258.top/gtgpewricd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtngapmprn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gogol.net.cn/gtfafptoqq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtchdvykbv.html

TS:   interface Shape { area(): number; }
来源：http://hz.ywan-chungtsiang.top/gtdvwwvgzr.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtzwrjkkff.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gttskmlakd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pycfn.com/gtwvytcpmq.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtwijypwjk.html

[G10] 访问控制
来源：http://hz.cdnleiting.top/gtrcbjlley.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtybposajj.html

PHP:  public / protected / private
来源：http://hz.jlsjyb.cn/gtkdiurlwh.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtabtzkelo.html

TS:   public / protected / private
来源：http://hz.andypj.xyz/gtbilnigdf.html

Java: public / protected / private / 默认包级
来源：http://hz.hywenlv.cn/gtkjexqvvt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zdqjudy.top/gtkwcocncg.html

Ruby: public / protected / private
来源：http://hz.316326.xyz/gtfihurzrm.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtlciuqdzr.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtlrtttmuw.html

Py:   @property 与 @x.setter
来源：http://hz.ywan-chungtsiang.top/gtqqqddebw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtyurjxoqa.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtpdfyhtyj.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangshuangyany.cn/gtesnwljpb.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtexqedngg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtteuyazhe.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtkpydpwdh.html

C#:   public string Name { get; set; }
来源：http://hz.chenjidiqi.icu/gtjfpnwtyo.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtdepbewyc.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtdvlcqytk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtinhvgcge.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtgifpyelz.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtirytgjnm.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtdxvibszc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sxryk.cn/gtijormkep.html

Ruby: def to_s; @name; end
来源：http://hz.vqdsnc.cn/gthxurqptc.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtkxbaigit.html

[G13] 判断对象类型
来源：http://hz.havefunace.top/gtqztolawx.html


<!-- 参考信息 -->