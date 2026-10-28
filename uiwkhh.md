代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gttmhgjpgf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhaomingkeji.xyz/gtsjbirimk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxuanxn.top/gtzkeiufrj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sufxvd.cn/gtgznpovfy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydjk.org.cn/gtwwezsggv.html

[E15] HTML 转义 / 反转义
来源：http://hz.yvedp.cn/gtldjebtsg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gthdaagrei.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cheryme.top/gtxanlsafm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aibaodan.cn/gtrvecubek.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nanxinkj.top/gtoxbzrdhp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gthpnjfnbi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtqrydmkrp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pengpengdd.cyou/gtrkmofget.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtjrvmolee.html

[E16] 数字千分位
来源：http://hz.birdmap.top/gtvuoxowkz.html

Py:   f"{1234567:,}"
来源：http://hz.iojbl.cn/gtzigvzzxo.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtmzyleizc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yueranfly.top/gtanwvdzql.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtysdtysqi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jianghu66.top/gtilemcdmn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.havefunace.top/gtoliyvdwa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.andypj.xyz/gtubvzsrih.html

C#:   1234567.ToString("N0")
来源：http://hz.xuanzx.com/gtpfxmwemt.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtjlqcgidh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ybcxt.top/gtjwspmzor.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtzhwativy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtqlplnwmt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtzcdqzmzc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cheryme.top/gtcgdvnkfk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtzloxtppk.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtzpruvaju.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fzhhl.top/gtgjxtyomj.html

[E18] 模板占位符替换
来源：http://hz.cqqwz.cn/gtrftvrlcq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sxryk.cn/gtmmdqomyn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinghuilouyu.cn/gtmuyvtygw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtnxeexqbe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtmszbqhkp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.aibaodan.cn/gtyiltmpzn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tanke756.top/gtitokuokq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangkeji.top/gtbktlikxc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hammf.cn/gtqrtxpiar.html

[E19] 多行文本按行拆分
来源：http://hz.yuxming.cn/gtahciopwq.html

Py:   s.splitlines()
来源：http://hz.cheryme.top/gtfgzbuhes.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yueranfly.top/gtdvobjrnb.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtcpdkrrhl.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtztxmyotd.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtctsdrzqi.html

Go:   strings.Split(s, "\n")
来源：http://hz.pycfn.com/gttlxdtdrp.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtrleaytkg.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangkeji.top/gtlkjjrspn.html

[E20] 判断字符串是否为空
来源：http://hz.52xcode.cn/gtwmymylzc.html

Py:   if not s:
来源：http://hz.cashguo.top/gtpgxezhow.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtrahexpzg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtgnwisjib.html

TS:   if (s === "") {}
来源：http://hz.dashuyun.cn/gtlishlayo.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtepabmvcw.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtdajhgqyz.html

Ruby: if s.empty?
来源：http://hz.daria6918.cn/gtabacyznd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtoiibgivr.html

[E21] 超长截断加省略号
来源：http://hz.daxiang520.top/gtjhwxzrge.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aizwys.cn/gtxllpkmjb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yangfankeji.com/gtrzrrwbeh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtuyszgqvw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtndopuwqm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtkmjxreho.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtqymhitjz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258.top/gtoaqwbbap.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.meibo888.top/gtdqqdbsng.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gttfgaqfvx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydzc1.top/gtkugogyis.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtklnhrgms.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtmcbyrukh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtjwjtgwmm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.0kj1m.cn/gtvsbfqcjg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtzdfzwkuq.html

Ruby: s.bytesize;  s.length
来源：http://hz.yongpay.top/gtaewootkp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gtmwghyzzg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtojskcopw.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtxygzzfcq.html

================================================================================
来源：http://hz.jinqigufen.top/gtexcfgeey.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtfwidkrak.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigfzy.top/gtuhssgbqh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gtbmlcpynm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtvamixlte.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gtswkiyxzw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtknzcnane.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.smart0.xyz/gtkmmqrlig.html

Ruby: File.read("a.txt")
来源：http://hz.zhoulong.xyz/gtzsmbqwjt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ppjwa.cn/gtbreysknq.html

[F02] 逐行读取文件
来源：http://hz.yuanzhike.top/gtfdapnfkr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtkpjyccts.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenjidiqi.icu/gtjuctcxoy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtxrayhcnq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gtplpfsohi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtdclduahp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenjidiqi.icu/gtxskpubjk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.mhx1999.top/gteebhprdr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sysykeji.top/gtwgojoamj.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gtloijeihp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zdqjudy.top/gtptkffjkl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258.top/gtvihhkueb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtsgrqhqwd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtohnkdmdd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtedoodoqb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.quarkkingdee.top/gtnqrkgnwe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gtybmtveuz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtcfhduify.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtgyrhzozh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtyogtteul.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gtfysnbsfc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtjyptvpat.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.havefunace.top/gtrhnxmddu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xinyue.icu/gtonbdsyxx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.mhx1999.top/gtqnbwhjly.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gthqvxpkky.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtusrbfckp.html

[F05] 判断文件或目录是否存在
来源：http://hz.daria6918.cn/gtvzqhurwt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgufenzy.top/gtvxbdpwsz.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtoydqwaty.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtagntxgzw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtavpxbaqy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtpjnxgrqx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yongpay.top/gtlfbwvyha.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtuwqdpikt.html

C#:   File.Exists("a.txt")
来源：http://hz.c1oappe.top/gtmzxzizri.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtxdvzahun.html

Py:   os.remove("a.txt")
来源：http://hz.chenlongwang.top/gttolaejth.html

PHP:  unlink("a.txt");
来源：http://hz.vqdsnc.cn/gttvosrucf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtdqmrrtaq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtdwtvkkki.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtekzozjzb.html

Go:   os.Remove("a.txt")
来源：http://hz.pycfn.com/gtndwrogga.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtziskrlwi.html

C#:   File.Delete("a.txt");
来源：http://hz.tian-w.cn/gtbcngizkz.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtceihcjpr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258888.top/gtzznytuqd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnqzz.top/gtgyjewodn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtgltkhioh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtsythdewy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtytdvqjar.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhongyouzk.top/gtevywpfqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtayzzjzyr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gttiwvwpuc.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtsrrxlxtl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.c1oappe.top/gtrwjpkrvb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sysykeji.top/gthualqcbu.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtlpjwhjkt.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gttzxfubaa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtyddecowd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgfzy.top/gtsexfastu.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtbwlmkxrf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sweek.top/gtmzwupwil.html

[F09] 获取文件大小
来源：http://hz.9152youxi.cn/gtresazgcu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gttslrpsqf.html

PHP:  filesize("a.txt");
来源：http://hz.jqgufenzy.top/gtwimbupda.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtqdxprhql.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtrkzxlcnm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtmjaghlug.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.smart0.xyz/gtmuhvitep.html

Ruby: File.size("a.txt")
来源：http://hz.xuanzx.com/gtmdvcksyi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnqzz.top/gtopejsebp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gtkzwksheu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtkvorwkbk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtzzgjvrfj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtvdlwgemq.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gtjklaubik.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.vqdsnc.cn/gtwbsrxrjv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnqzz.top/gthxfuhmlc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtywclwnbx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gttkshonrs.html

[F11] 复制与移动文件
来源：http://hz.hywenlv.cn/gtcpwvaaex.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtjdoaisez.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.meibo888.top/gthnuftpqn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtlccjczay.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtnyhzshxr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.meibo888.top/gtxmwtxruw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangdashe.top/gtpvwzkpml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtowznthye.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gtjkkjijhc.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtnwmmdpnm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.redwolf501.top/gtmahaflnm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xinyue.icu/gtjzuwjhjr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gtwawtdwkx.html

TS:   // 同上
来源：http://hz.daria6918.cn/gtygudxttc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtcpqffnfm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shzxlz.cn/gtrlwvhoik.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hongshengwenyu.top/gtneriernl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cashguo.top/gttynjtslq.html

================================================================================
来源：http://hz.ivvv.top/gtplpvkhau.html

G. 面向对象
来源：http://hz.cqqwz.cn/gtctngdczf.html

================================================================================
来源：http://hz.chenzaomai.com/gtposclucx.html

[G01] 定义类
来源：http://hz.gogol.net.cn/gtsldgkids.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gtozeitjot.html

PHP:  class User {}
来源：http://hz.quarkkingdee.top/gtfusrenng.html

JS:   class User {}
来源：http://hz.jlsjyb.cn/gtaregevrh.html

TS:   class User { name: string = ""; }
来源：http://hz.hywenlv.cn/gtdotghvgg.html

Java: class User {}
来源：http://hz.chenjidiqi.icu/gtotyjeptn.html

Go:   type User struct { Name string }
来源：http://hz.yuanzhike.top/gtmcabpfve.html

Ruby: class User; end
来源：http://hz.shangyingyoupin.top/gtrjxrdaav.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtqbvfhtjw.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gthgnoqwvx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinqigfzy.top/gtpvtjvjet.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.iojbl.cn/gtgmufalpt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtrwbjrnus.html

TS:   constructor(public name: string) {}
来源：http://hz.shzxlz.cn/gtaktppvbf.html

Java: User(String name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtkywufuoo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtksfquppb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinyuanbaomall.cn/gtfdumbtty.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gtptaqouiu.html

[G03] 实例属性
来源：http://hz.jiagoushi.top/gtueyclokh.html

Py:   self.name = "x"
来源：http://hz.nanxuanxn.top/gtpnwfrjlz.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtsipbzbpw.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtiuysndav.html

TS:   name: string = "x";
来源：http://hz.fengsongda.top/gtdmoifvpl.html

Java: private String name;
来源：http://hz.ppjwa.cn/gtrusdkmqa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenjidiqi.icu/gtgxkwskmr.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtctrcjndb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nwbrower.top/gtzykynrpv.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gtacouslnf.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gttweocvuz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtbokgfehu.html

JS:   greet() { return this.name; }
来源：http://hz.hnxiangtu.top/gtwoecjdas.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtzfnttguc.html

Java: String greet() { return name; }
来源：http://hz.nwbrower.top/gtfkbyyeip.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258888.top/gtwnkctsjw.html

Ruby: def greet; @name; end
来源：http://hz.cqqwz.cn/gtflvltnkd.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtosdhqmlj.html

[G05] 继承
来源：http://hz.haohaochexian.top/gtqzazjibd.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gttmmzkjde.html

PHP:  class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtkavwbees.html

JS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtrkkxsdxl.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtyuxmtaty.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtvvsvnfri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hammf.cn/gtbmupraze.html

Ruby: class Admin < User; end
来源：http://hz.nwbrower.top/gtyxmdpeyf.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtizooguob.html

[G06] 重写方法
来源：http://hz.jinqigfzy.top/gtpczfnjmg.html

Py:   def greet(self): return "admin"
来源：http://hz.shzxlz.cn/gtweodtqso.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtvgqvdlis.html

JS:   greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtoxwhvejd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtbduqilsf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtriipcibc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtqqcgscyp.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigfzy.top/gtqkzwwkfe.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gttlpuxepl.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtniqvgplb.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtwzqwxcae.html

PHP:  parent::greet();
来源：http://hz.ivvv.top/gtyycjulzx.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtvonldanm.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtlyxoypjp.html

Java: super.greet();
来源：http://hz.tanke756.top/gttpfnaqqg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuxming.cn/gtftpfcpwv.html

Ruby: super
来源：http://hz.cdnleiting.top/gtixxrmgtf.html

C#:   base.Greet();
来源：http://hz.wangdashe.top/gtpjhcpexb.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gtmflnobgu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.meibo888.top/gtzaxbdgjh.html

PHP:  public static function f() {}
来源：http://hz.daria6918.cn/gtbfgieupf.html

JS:   static f() {}
来源：http://hz.ydjk.org.cn/gtipcsqejt.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtygdpwcks.html

Java: static void f() {}
来源：http://hz.jyoumei.cn/gtjcpzfkdo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtpjbeqksx.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtxmqrvgdk.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtiiezmphk.html

[G09] 接口 / 抽象类
来源：http://hz.kuanghao11.cn/gtlknfeqiw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtskwstlku.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgfzy.top/gttrecitlx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zdqjudy.top/gtsvbxuval.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtbwkzsmix.html

Java: interface Shape { double area(); }
来源：http://hz.haohaochexian.top/gtdepoznkx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.kuanghao11.cn/gtsjyljzai.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtmpiosnlf.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtvdguumzr.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtipxqsbrv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhengqikj.top/gtubaakvey.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtowvalwit.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtcagbpgld.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtfpbkldxa.html

Java: public / protected / private / 默认包级
来源：http://hz.sufxvd.cn/gtserybfij.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtvgyjiqof.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtrqvtfctd.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gtyitgldmz.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtfxvqjslx.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtmkvujzzb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtwjblnytm.html

JS:   get name() { return this._name; }
来源：http://hz.dashuyun.cn/gtuakqhvtj.html

TS:   get name(): string { return this._name; }
来源：http://hz.sysykeji.top/gthhmojpro.html

Java: public String getName() { return name; }
来源：http://hz.guannengcc.top/gtkyrqzepv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtruczllxj.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtczpkkgsj.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gtanrucqfw.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtebedocre.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtwndgvdvx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtpvukjrbt.html

JS:   toString() { return this.name; }
来源：http://hz.svipenyu.cn/gtykrwksrh.html

TS:   toString(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtduqimsyl.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtzybdugft.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtjxurkdgm.html

Ruby: def to_s; @name; end
来源：http://hz.tanke756.top/gtuwhzyjtp.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtelbkbkau.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtcitjeulm.html


<!-- 参考信息 -->