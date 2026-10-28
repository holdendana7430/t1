代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dashuyun.cn/gtmnhwutff.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtrjudlscm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yongpay.top/gtsryicbgx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnqzz.top/gtjngzfxbk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gtndmeabzn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtrxfwewkn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.kuanghao11.cn/gtnrhbsxjh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nwbrower.top/gtbswcykin.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cdnleiting.top/gtljvbeooc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangtech.top/gtexurllpt.html

[E16] 数字千分位
来源：http://hz.tianlin.xyz/gtdomcnbav.html

Py:   f"{1234567:,}"
来源：http://hz.yuxming.cn/gtdtuwpdnb.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtmernfnbu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtcobwbmux.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtragwwhjh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yueranfly.top/gteqnivwel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnqzz.top/gtgvwhxial.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtcwwevyga.html

C#:   1234567.ToString("N0")
来源：http://hz.cqqwz.cn/gtscfgugif.html

[E17] 首字母大写
来源：http://hz.ehwqpu.com/gtihdhdfsj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxinkj.top/gtzeqpmmxq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hysaishi.cn/gtxcezqbxh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtqlcqfabj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtwynojpcp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtcoclqsud.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cheryme.top/gtptkqsvvd.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtyamgzvgc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxuanxn.top/gtpyqibgcf.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gttecrpuee.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.birdmap.top/gtbppnaehn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.feifeiyinyue.top/gtzrlqpfmj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtelrmqhjw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtizlocnfg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zdqjudy.top/gtkhgppliw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtqynkibab.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gaohongyu789.top/gttadlfvii.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxinkj.top/gtxdcnhuwz.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtftxsrose.html

Py:   s.splitlines()
来源：http://hz.jiagoushi.top/gtunmtqiwg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxinkj.top/gtzcmhsyde.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtivymefrx.html

TS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtglzbemwr.html

Java: s.lines().toList()
来源：http://hz.chenjidiqi.icu/gtjomiabzo.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhaomingkeji.xyz/gtfggymttk.html

Ruby: s.lines
来源：http://hz.gaohongyu789.top/gtvjycvehx.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtgevhtxkg.html

[E20] 判断字符串是否为空
来源：http://hz.tian-w.cn/gtphtwaryo.html

Py:   if not s:
来源：http://hz.gaohongyu789.top/gtmdtrtpzi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtiezfsrjn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtpokcbgnn.html

TS:   if (s === "") {}
来源：http://hz.nwbrower.top/gtmsuambzt.html

Java: if (s.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtizdxoncv.html

Go:   if s == "" {}
来源：http://hz.shangyingyoupin.top/gtynfdvnkq.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtzvlpghuk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hnqzz.top/gtkdlcnzlf.html

[E21] 超长截断加省略号
来源：http://hz.haohaochexian.top/gtpljqheyu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtteijvjvq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtylfteahb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtccrhjyel.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtygeehmrp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gthjxmspce.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtcpaqmeuv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cdnleiting.top/gtuoxirfgf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtaosbrrgj.html

[E22] 字节长度与字符长度
来源：http://hz.yonumen.top/gtbzdgqard.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yongpay.top/gtkrynsylh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtymautidq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gthviejidv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hammf.cn/gtlgxpnsmr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gotoacloud.top/gtdoikrgzu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.feifeiyinyue.top/gtsgwjlitr.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gtuaqotdss.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtiyrmsivo.html

================================================================================
来源：http://hz.jqgfzy.top/gtvcggwsud.html

F. 文件与目录
来源：http://hz.quarkkingdee.top/gtvufnjaxx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtyimvcjnx.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtkjicmhbz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cashguo.top/gtmzjoxerq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtvgpshwpp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gtalqvodga.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daria6918.cn/gtuxwjhihr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtjofemplp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gtckwasoyb.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtjamaxizs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangtech.top/gtpwyuvtgq.html

[F02] 逐行读取文件
来源：http://hz.xinyue.icu/gtutkwgaft.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtpyurdhuo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tanke756.top/gtuqtnzwxq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtwmwusxoh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gttkdviobe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtsskmcjgh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtzlilaraa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gteovkvdca.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.redwolf501.top/gtippzegxx.html

[F03] 写入文件（覆盖）
来源：http://hz.aizwys.cn/gttuvmpjuw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yangfankeji.com/gtddldgigf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtasqfniao.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.iojbl.cn/gtkmhrxgiw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gthorhvryj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtycsbmiil.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zycfv.cn/gtmyobjxlw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gtcrrvaobi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtfpzdkhkm.html

[F04] 追加写入文件
来源：http://hz.xuetiantiany.cn/gtgifrqtdt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtkmablbhv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fengsongda.top/gtxkxjihva.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtqbsteman.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtoxaaxtck.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xziqi.cn/gtyztqosvw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ywan-chungtsiang.top/gthrldeweu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydjk.org.cn/gtlyqeujel.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtcyuvyxgo.html

[F05] 判断文件或目录是否存在
来源：http://hz.gaohongyu789.top/gtcnbtabbq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hfpthk.cn/gtegqlcvot.html

PHP:  file_exists("a.txt");
来源：http://hz.pengpengdd.cyou/gtwfoflbgk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtawrpzkha.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtgiodgbil.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtrsfrgzyj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.redwolf501.top/gtedkfcibc.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gthmwvabdh.html

C#:   File.Exists("a.txt")
来源：http://hz.jinghuilouyu.cn/gteellstuk.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gtnuzpoyjr.html

Py:   os.remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtuwwfpgxq.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258888.top/gtxhsjydkb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtfemvfrbl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtlqutxhaj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gticbxrhue.html

Go:   os.Remove("a.txt")
来源：http://hz.guowangkeji.top/gtcvquikvr.html

Ruby: File.delete("a.txt")
来源：http://hz.dashuyun.cn/gtvtzeslmk.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangtech.top/gtejnexgzo.html

[F07] 创建目录（含多级）
来源：http://hz.snrcjt.cn/gtpnbxmnvg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtoxdatozs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gtffhszarz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtztsefkwp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gthgpkfrxg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtuxtlusys.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.bjfxy.top/gtinbrlsll.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pengpengdd.cyou/gttzjrziky.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fzhhl.top/gtbpgnjeet.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gtryuxtvxl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtgjtitatf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtetevuohl.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtfycmhzif.html

TS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gteetpewck.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtlpwtoehs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtwehldigk.html

Ruby: Dir.children("dir")
来源：http://hz.cheryme.top/gtluebhfcb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtywlivxsl.html

[F09] 获取文件大小
来源：http://hz.birdmap.top/gtmiiawtqk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtosmjfexa.html

PHP:  filesize("a.txt");
来源：http://hz.wangdashe.top/gtnsxskabe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtnmgudyxx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtvyqqfypr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtowupgmde.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gtzblwlhlo.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtrqcqjlvl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.kuanghao11.cn/gtqxumihql.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangshuangyany.cn/gtcqjhbzxi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtfyqntsji.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.bjfxy.top/gtloaphpna.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtewjwvmun.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtflzxhahe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxinkj.top/gtnagzcoej.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtmrmuozcm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtncxevymx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtjtlafiqn.html

[F11] 复制与移动文件
来源：http://hz.cheryme.top/gtlgqulnow.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtrjuwvciq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinghuilouyu.cn/gtcseskxyx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gttnvlsqou.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtlvqxrbwr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shuidangran.top/gtwclecgqv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.smart0.xyz/gtgzgpbhav.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtdtezwvfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtwjylrptr.html

[F12] CSV 读写
来源：http://hz.cheryme.top/gtyobbzbij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hywenlv.cn/gtqvekcdin.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tanke756.top/gtdpuxasjo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dianchejie.cn/gtwxekkiwj.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtkdheapwq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgufenzy.top/gtmnelkote.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuxming.cn/gtzzvrxucg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxuanxn.top/gtupvuxplu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gogol.net.cn/gtzjcsidok.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxegahyrc.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtojfoayjn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwwldwpfa.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtazkcgdgj.html

Py:   class User: pass
来源：http://hz.shanyushiyangtech.top/gteguzpzjn.html

PHP:  class User {}
来源：http://hz.yuxming.cn/gtrxkszibn.html

JS:   class User {}
来源：http://hz.ivvv.top/gtdynsubhs.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtlozcuyms.html

Java: class User {}
来源：http://hz.jinqigufen.top/gtuzmwjsio.html

Go:   type User struct { Name string }
来源：http://hz.wangdashe.top/gtuxsqbizh.html

Ruby: class User; end
来源：http://hz.daria6918.cn/gtnajnwixc.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtypivovfs.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtfrpfpmxn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtbeivpqfr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yanxiufei.cn/gttxgkbgra.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtiypudyhb.html

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gtvnsfyhac.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtitjamwwj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhongyouzk.top/gtptnngaqw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xingfuxueyuan.xyz/gttmzcllnv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ybcxt.top/gtgylrvezl.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtmygxkyfr.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtinifesac.html

PHP:  public string $name = "x";
来源：http://hz.fzhhl.top/gtvrlzzlqw.html

JS:   this.name = "x";
来源：http://hz.ehwqpu.com/gtdjknrzym.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtttegdfjz.html

Java: private String name;
来源：http://hz.svipenyu.cn/gteuhpfdqi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtfzuqdkrq.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtouimoyzu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtjzmqvodc.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtvupcfzio.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtofnxsbas.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtjmuqghgr.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtsbuoigfp.html

TS:   greet(): string { return this.name; }
来源：http://hz.yvedp.cn/gtqwnradlh.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtjvxsbrpl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.52xcode.cn/gtegcfpvwx.html

Ruby: def greet; @name; end
来源：http://hz.haohaochexian.top/gtcijwwaly.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gtclcggkgb.html

[G05] 继承
来源：http://hz.yj202588.top/gtfuzfncsf.html

Py:   class Admin(User): pass
来源：http://hz.yongpay.top/gtgqwtcnok.html

PHP:  class Admin extends User {}
来源：http://hz.sufxvd.cn/gtornlngcz.html

JS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gthaiqfyha.html

TS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtzbwnnoxt.html

Java: class Admin extends User {}
来源：http://hz.pycfn.com/gtolxewyjp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hammf.cn/gtqdlangdp.html

Ruby: class Admin < User; end
来源：http://hz.c1oappe.top/gtbuiiakos.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtwjxshion.html

[G06] 重写方法
来源：http://hz.dianchejie.cn/gtlutqompn.html

Py:   def greet(self): return "admin"
来源：http://hz.shzxlz.cn/gthluyqltf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtrozphnav.html

JS:   greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtbjsrgvcn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtlsdidpoa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtyvsbaqxm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtwzkopynh.html

Ruby: def greet; "admin"; end
来源：http://hz.cashguo.top/gtaqjzhwdp.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtpvrbfido.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtrxyhaaks.html

Py:   super().greet()
来源：http://hz.hywenlv.cn/gtizgtysbu.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtakzqmhxb.html

JS:   super.greet();
来源：http://hz.ehwqpu.com/gtjgjqymqm.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtquausdey.html

Java: super.greet();
来源：http://hz.zhoulong.xyz/gtzringzmb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtdophvdzr.html

Ruby: super
来源：http://hz.xziqi.cn/gtealabpjc.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtqndlsays.html

[G08] 静态方法与属性
来源：http://hz.cqqwz.cn/gtgeeivdki.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.0kj1m.cn/gtbnqorbrv.html

PHP:  public static function f() {}
来源：http://hz.ywan-chungtsiang.top/gtafazslyv.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gttgtxgaul.html

TS:   static f(): void {}
来源：http://hz.chenzaomai.com/gtxyxxahcw.html

Java: static void f() {}
来源：http://hz.cdnleiting.top/gtqckrhdtn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hfpthk.cn/gtorvlxhxs.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtuulvvzlc.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gtclxfqqsh.html

[G09] 接口 / 抽象类
来源：http://hz.ydjk.org.cn/gtuciyjsxq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtuewjnixk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.mhx1999.top/gttzsoskrb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.svipenyu.cn/gtoudfwtnt.html

TS:   interface Shape { area(): number; }
来源：http://hz.tian-w.cn/gtntaeipoj.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtoffhqcqn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydzc1.top/gtmgyfzjpx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ivvv.top/gtklqodjyg.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtserbkdxl.html

[G10] 访问控制
来源：http://hz.iojbl.cn/gtoswllzew.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtkxtjwhak.html

PHP:  public / protected / private
来源：http://hz.jqgfzy.top/gteepdtond.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gtskxksicv.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gtxtkoxrsy.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gtelbazbyr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhongyouzk.top/gtlgrejmfi.html

Ruby: public / protected / private
来源：http://hz.52xcode.cn/gtiihubwac.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtqmqvpbta.html

[G11] getter / setter
来源：http://hz.zhixingplan.top/gtvuyvxquz.html

Py:   @property 与 @x.setter
来源：http://hz.guannengcc.top/gtplumnqaf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtulhrewem.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gthonsdutg.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhijiandao.cn/gtgoseyzpi.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gtvmkfkhon.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtkkqtfpdb.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtwtkawuio.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtynoeuowh.html

[G12] 对象转字符串
来源：http://hz.bjfxy.top/gtwaegqzgw.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtqovkthcp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtmznxfyfx.html

JS:   toString() { return this.name; }
来源：http://hz.sweek.top/gtcbnhvqnk.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtgiwjlurx.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtvmwpnjnk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtmxkmoupn.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gtkvjzwdtg.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigfzy.top/gtkbnfkivv.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gthfzyllei.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gtvgidwbyx.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtgzrfesub.html

JS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtlrrfyjdm.html

TS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtyluyghln.html


<!-- 参考信息 -->