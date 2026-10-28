代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.snrcjt.cn/gtqpuuxppx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtyzvajgrj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gthafacdtm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtrvjdtgma.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.mhx1999.top/gtchdrtknp.html

[E15] HTML 转义 / 反转义
来源：http://hz.316326.xyz/gtqwhklria.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhiwuduotai.top/gtnaivhxbl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gtdsvxshap.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cashguo.top/gtojppdbbg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtmyofdkjk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhoulong.xyz/gtxyvmhpnj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gtjqclaver.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jlsjyb.cn/gtpwsozkxc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.vqdsnc.cn/gtvjmnimqq.html

[E16] 数字千分位
来源：http://hz.meibo888.top/gtcafkxjjl.html

Py:   f"{1234567:,}"
来源：http://hz.ppjwa.cn/gtinpuykcv.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtyrgmhxmq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtmzebniyg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtqkwmcatg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sweek.top/gtgjuemibn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtcrimfzgt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xuetiantiany.cn/gtsbtitilz.html

C#:   1234567.ToString("N0")
来源：http://hz.xylfe.cn/gthmdjgaye.html

[E17] 首字母大写
来源：http://hz.gogol.net.cn/gtjihxknkt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtgkxhyecn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtcvbaytcn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtpzpwcumm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtvxsgdtbx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.vqdsnc.cn/gtjljnuzvz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinyuanbaomall.cn/gtberbtrst.html

Ruby: s.capitalize
来源：http://hz.guowangkeji.top/gtvadmkaut.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhaomingkeji.xyz/gtzopirdbz.html

[E18] 模板占位符替换
来源：http://hz.ybcxt.top/gtyghkqqxp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jiagoushi.top/gtjmqmrrhn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gthtlnmnfa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtonwejxjc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtwttpnjup.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtptgrqbmm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtmrtzefgq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhongyouzk.top/gtozegewpo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtoadjyhph.html

[E19] 多行文本按行拆分
来源：http://hz.jianghu66.top/gtaufxcgxh.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtlpzrqkcm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258888.top/gtvlqxgvto.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtfzetshtd.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtrxzmncej.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gtuaacbbyd.html

Go:   strings.Split(s, "\n")
来源：http://hz.sxryk.cn/gtojituqyo.html

Ruby: s.lines
来源：http://hz.jqgufenzy.top/gthcnwuaob.html

C#:   s.Split('\n')
来源：http://hz.jqgfzy.top/gtyokejfxu.html

[E20] 判断字符串是否为空
来源：http://hz.dianchejie.cn/gttlrctoll.html

Py:   if not s:
来源：http://hz.xingfuxueyuan.xyz/gtlxzuhnfx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtguvuxcor.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cucudq.cn/gtwldicswq.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtslvpurwn.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258888.top/gtquowyxra.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtzsyduhmz.html

Ruby: if s.empty?
来源：http://hz.yuxming.cn/gtwhtpmnug.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtwtaexcej.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtwubxtmms.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gtcsrygshg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtnokvhgxe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtxkqtxwso.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtwhihbxkt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtcgsfsryt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daxiang520.top/gtrstqvlri.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.redwolf501.top/gtymiblysx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.andypj.xyz/gtabtkhcsc.html

[E22] 字节长度与字符长度
来源：http://hz.zhiwuduotai.top/gtiqcsfwnu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yanxiufei.cn/gtskemxbca.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gticuhrrcp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtzjmwwqmt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gthdcfgkjx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtwaptoouf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gtcghkbgma.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gthnjlrosl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtjqwgpdjy.html

================================================================================
来源：http://hz.zhoulong.xyz/gtflrmlgvc.html

F. 文件与目录
来源：http://hz.yj20258.top/gttityddfz.html

================================================================================
来源：http://hz.nanxinkj.top/gtoaogehky.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtrxogjblb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtopuwzdsy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtmjjjqefr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtjudbfgej.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shuidangran.top/gtoigcslzy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtiheibgti.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtiiwpflhv.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtndzwqcxh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jlsjyb.cn/gthodalgsc.html

[F02] 逐行读取文件
来源：http://hz.yj20258888.top/gtimzjfvhc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gtxpuqvoio.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtvfvjhfxz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtvhucykoz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtbhzqufwn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtxloznkee.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtilzxbump.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gogol.net.cn/gtpozxqpsx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigufen.top/gtiqovrojh.html

[F03] 写入文件（覆盖）
来源：http://hz.yuanzhike.top/gtsnxycvyk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daria6918.cn/gtqxrhxvco.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtxqwlikaa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtzzuiafrh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtmnvrpvrc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtrokgbcxj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gzhubu.top/gtoljukkss.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gttjyrewwj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gthgqfldle.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtsahsxweo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.havefunace.top/gtkhjwjwus.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cheryme.top/gtbrcthgmr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtmewqueju.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtybrizlhe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daria6918.cn/gtalquyrrf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jiagoushi.top/gtbyeqkqxi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ppjwa.cn/gtcxdjxkhh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guowangkeji.top/gtdpcsnloa.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gtyimnanxg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gaohongyu789.top/gtiuwnibww.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtfigrydxv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gthurtaonb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gttzlutuau.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtydkiqltc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.havefunace.top/gtpgrermgq.html

Ruby: File.exist?("a.txt")
来源：http://hz.jlsjyb.cn/gtptkuqpbq.html

C#:   File.Exists("a.txt")
来源：http://hz.hammf.cn/gtxuegpluq.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtjyssefst.html

Py:   os.remove("a.txt")
来源：http://hz.sufxvd.cn/gtzpclmjbp.html

PHP:  unlink("a.txt");
来源：http://hz.jlsjyb.cn/gtscbyxapy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtscczudqd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtzfdxauii.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtxrxsspqx.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gthidakwiq.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtefxklqnq.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtqrncopce.html

[F07] 创建目录（含多级）
来源：http://hz.daria6918.cn/gtfoptvara.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aibaodan.cn/gtzmshcilh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuanzx.com/gtkoxmazpk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gthkiolpmx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtofkirtjp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhijiandao.cn/gtzxtgdfeq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtrqfliaxh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtckfccnhi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtwvwbowrl.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtdcrpjhqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daria6918.cn/gtobpbjshr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shanyushiyangkeji.top/gtkqmtjhnw.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtrfkwvkcx.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gttpyzbozi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gteqmjdlqr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gtyzaeomos.html

Ruby: Dir.children("dir")
来源：http://hz.ivvv.top/gtulsapqxs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtmqxkszke.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gtdvnldjvk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gtykcjhrkj.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtoywwzijc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtlgzdvdrb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtblqvncdi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtqbidfzej.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.mhx1999.top/gtczhaqwrz.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtcaovgzdx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.iojbl.cn/gtslibhxpp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtojsoxmkw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtvydiaweq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gtsgskgwev.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtgqrjlpua.html

TS:   path.extname("a.txt")
来源：http://hz.jlsjyb.cn/gtlfnpxooz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhongyouzk.top/gtevodpqvy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daxiang520.top/gtaoocdjqr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtglmwwgfr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xinyue.icu/gttevocoke.html

[F11] 复制与移动文件
来源：http://hz.yj20258.top/gtzagtjhbk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtpfiwfdjh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtxpknjzvf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtgeeuggvm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtxriyfdef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guannengcc.top/gtqjiyxmrw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.kuanghao11.cn/gtoaiwlaot.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gttalxjezv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.snrcjt.cn/gtqjuacjnh.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gtjrboxwma.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aibaodan.cn/gthltrpbde.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtdwexfptt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtrrkrpmia.html

TS:   // 同上
来源：http://hz.daria6918.cn/gtrwzcwkaa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtjtscnrxu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.snrcjt.cn/gtwpygjolg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fengsongda.top/gtcjgsqxan.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gttjescnex.html

================================================================================
来源：http://hz.9152youxi.cn/gtvgmdjuun.html

G. 面向对象
来源：http://hz.xziqi.cn/gtvkhoujfk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkxnmpowy.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtepbjwfaq.html

Py:   class User: pass
来源：http://hz.jinyuanbaomall.cn/gtnwhwvmoz.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtqbivudvf.html

JS:   class User {}
来源：http://hz.guowangkeji.top/gthlorrolh.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gtygpvnlhl.html

Java: class User {}
来源：http://hz.iojbl.cn/gtimgxcvyz.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gttxgdbyam.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gthtuzwppj.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gtoubsuhcl.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtmgsuactv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.0kj1m.cn/gtakhqrpva.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hammf.cn/gttsrdhyyh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shuidangran.top/gtvlnsussy.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gtxxmhpifg.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuxming.cn/gtpanxuxhb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtdvtgohii.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtkdwzlklf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gthkeykeuw.html

[G03] 实例属性
来源：http://hz.ydjk.org.cn/gtejtdwrhc.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gthabjkdrs.html

PHP:  public string $name = "x";
来源：http://hz.redwolf501.top/gtvimaxcrx.html

JS:   this.name = "x";
来源：http://hz.0kj1m.cn/gtasteoxon.html

TS:   name: string = "x";
来源：http://hz.gotoacloud.top/gtjgguxehd.html

Java: private String name;
来源：http://hz.yuanzhike.top/gtaqzllmdd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtloueuvua.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gtyvfpjrxo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangdashe.top/gtpyfxodzf.html

[G04] 定义方法
来源：http://hz.shzxlz.cn/gtxyvhwvde.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtwwmkuybl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtrtgbmxgf.html

JS:   greet() { return this.name; }
来源：http://hz.9152youxi.cn/gtxsijhokz.html

TS:   greet(): string { return this.name; }
来源：http://hz.tian-w.cn/gtrwwaditt.html

Java: String greet() { return name; }
来源：http://hz.jinqigfzy.top/gtmepmecsa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hywenlv.cn/gtsduahggx.html

Ruby: def greet; @name; end
来源：http://hz.c1oappe.top/gtaoruufyi.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtwjyfrutz.html

[G05] 继承
来源：http://hz.haohaochexian.top/gtjheoyefi.html

Py:   class Admin(User): pass
来源：http://hz.cdnleiting.top/gtqxbzkrqj.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtflettyin.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtszyvbptw.html

TS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtekjtajjy.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtppbjjgvn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtcnqwcosw.html

Ruby: class Admin < User; end
来源：http://hz.sweek.top/gtazvnqzkq.html

C#:   class Admin : User {}
来源：http://hz.birdmap.top/gtfrfznhpa.html

[G06] 重写方法
来源：http://hz.zhaomingkeji.xyz/gtswloiakf.html

Py:   def greet(self): return "admin"
来源：http://hz.yongpay.top/gtvbittnfl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtkcnztldn.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gticlynxlk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtidvocyvd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtbgrbviev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhixingplan.top/gttmtskomt.html

Ruby: def greet; "admin"; end
来源：http://hz.cashguo.top/gtcseqgyis.html

C#:   public override string Greet() => "admin";
来源：http://hz.iojbl.cn/gtbmxzhakq.html

[G07] 调用父类方法
来源：http://hz.feifeiyinyue.top/gtrmrpsyup.html

Py:   super().greet()
来源：http://hz.wangdashe.top/gtxgeiijjd.html

PHP:  parent::greet();
来源：http://hz.haohaochexian.top/gtsljtdqfa.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtdjfcuzsm.html

TS:   super.greet();
来源：http://hz.hfpthk.cn/gtofjxgfdd.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtqbzecyum.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guowangkeji.top/gtvseipoqc.html

Ruby: super
来源：http://hz.nanxuanxn.top/gtznbwzzif.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtzaxlnpfp.html

[G08] 静态方法与属性
来源：http://hz.bjfxy.top/gtrdnwrvsz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtkxguafax.html

PHP:  public static function f() {}
来源：http://hz.jinghuilouyu.cn/gtzxaldhoq.html

JS:   static f() {}
来源：http://hz.ybcxt.top/gtfwbcfuhf.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gtqyrnovyy.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtnqrentuw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.meibo888.top/gtvovjpdgv.html

Ruby: def self.f; end
来源：http://hz.cucudq.cn/gteuffznub.html

C#:   public static void F() {}
来源：http://hz.nwbrower.top/gtlpwmkmrz.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtlztzjrtu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtwlogurwm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtiknisbol.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aibaodan.cn/gtkgbacimz.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtoqlccmyc.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gthpttdsio.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtueueymog.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtwquzivdp.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtalrbyzhy.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtjameyfhh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.kuanghao11.cn/gtciaohtbv.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gtlceomssp.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtfmvpyeir.html

TS:   public / protected / private
来源：http://hz.sufxvd.cn/gtecqzhtyc.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gtzayhorbv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.9152youxi.cn/gtllwoiegt.html

Ruby: public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtijwstaow.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtcrmkdiqt.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtsnewenvr.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtgtihiaiu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtnwmcmhjf.html

JS:   get name() { return this._name; }
来源：http://hz.chenjidiqi.icu/gtgigwacto.html

TS:   get name(): string { return this._name; }
来源：http://hz.yonumen.top/gtplvfkzrn.html

Java: public String getName() { return name; }
来源：http://hz.ehwqpu.com/gtxwibrnle.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hysaishi.cn/gtgrkmxwze.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtwcmezlsi.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtggoflcpg.html

[G12] 对象转字符串
来源：http://hz.vqdsnc.cn/gtewhevblf.html

Py:   def __str__(self): return self.name
来源：http://hz.aibaodan.cn/gtltcxhcmf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtywwvwmax.html

JS:   toString() { return this.name; }
来源：http://hz.c1oappe.top/gtgwtkxkca.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtlvcukbhz.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtebcsmgko.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yongpay.top/gtahipngrc.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtzvdplqul.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gthkskzvhu.html

[G13] 判断对象类型
来源：http://hz.gzhubu.top/gtsjogfjti.html


<!-- 参考信息 -->