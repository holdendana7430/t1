代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gaohongyu789.top/gtdxtsksba.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtdiwldcvq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtlvkbovqk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dashuyun.cn/gtocrmfvyq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aizwys.cn/gteweqftfp.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenlongwang.top/gtewnljard.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dianchejie.cn/gtyojhnsqd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtecgeunwu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dianchejie.cn/gttelczsig.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sysykeji.top/gtbxkopvsk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yanxiufei.cn/gtsiuhqfka.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtjeepdnnz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gtpkiloket.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtglquackk.html

[E16] 数字千分位
来源：http://hz.gaohongyu789.top/gtmrcijcye.html

Py:   f"{1234567:,}"
来源：http://hz.xuetiantiany.cn/gtfcfwxeuo.html

PHP:  number_format(1234567);
来源：http://hz.jiagoushi.top/gtkloepbkr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xziqi.cn/gtdbtcahyl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtizacxnte.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sxryk.cn/gthmyaxmcx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgufenzy.top/gtcgpflpgu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jianghu66.top/gtizrtqzmr.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtoyrbyecn.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtalzqgtzg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangtech.top/gtbrgionnw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxinkj.top/gtljwworea.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtimvpslmc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtbfkiqadc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gteynuvlzk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gtuuwvlwqj.html

Ruby: s.capitalize
来源：http://hz.iojbl.cn/gtwfhkvbck.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nwbrower.top/gtjinapvnt.html

[E18] 模板占位符替换
来源：http://hz.birdmap.top/gthnqcjlpp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgfzy.top/gtfssalbka.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gtewkkiayl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtjqhaafgl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gtyemviywe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gtcgyhicuy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sysykeji.top/gtxkhushqn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtntkpwili.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhoulong.xyz/gtosxkliiv.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtzammhqqc.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtqirxkqru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gtivxfobnm.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtzgqgsspd.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtqtpcvfvx.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtejljrqtf.html

Go:   strings.Split(s, "\n")
来源：http://hz.hongshengwenyu.top/gtvwusexwe.html

Ruby: s.lines
来源：http://hz.chenjidiqi.icu/gtqwpdcadr.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtavtyofpr.html

[E20] 判断字符串是否为空
来源：http://hz.zhiwuduotai.top/gthakibsbd.html

Py:   if not s:
来源：http://hz.yuanzhike.top/gtaocfnwie.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhixingplan.top/gtadaxefki.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daria6918.cn/gtnmojwavu.html

TS:   if (s === "") {}
来源：http://hz.hfpthk.cn/gtlqmsfrtn.html

Java: if (s.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtreyywvus.html

Go:   if s == "" {}
来源：http://hz.jqgfzy.top/gtgbksjolo.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtincikbnn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.bjfxy.top/gtuxvuajyw.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtueamrbid.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gogol.net.cn/gthwrrzbtl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgufenzy.top/gtwytollri.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtfcvtkwjl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtjadlzcww.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtqfleubxb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gtyjrsvdud.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhijiandao.cn/gtxaludorn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtxhksbmvm.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gthazbkmtb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.haohaochexian.top/gtwanviwvb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtfyylkwvb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gthydvakns.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtbnzzpepv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtouswswhr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shangyingyoupin.top/gtlusqfbpr.html

Ruby: s.bytesize;  s.length
来源：http://hz.redwolf501.top/gtsxnqwwca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuxming.cn/gtmwjmiayn.html

================================================================================
来源：http://hz.zhijiandao.cn/gteqgicrdg.html

F. 文件与目录
来源：http://hz.havefunace.top/gtpmrhwdiw.html

================================================================================
来源：http://hz.dianchejie.cn/gttuvmbjwm.html

[F01] 读取整个文件
来源：http://hz.zycfv.cn/gtzjlvrlcl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gtadublfcj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guowangkeji.top/gtpdrattea.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtulhqkzud.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtixtzghga.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtaevgrxky.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtyflvpcav.html

Ruby: File.read("a.txt")
来源：http://hz.guannengcc.top/gthntiadin.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.iojbl.cn/gtymwyoegn.html

[F02] 逐行读取文件
来源：http://hz.nanxinkj.top/gtgjhhofos.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenzaomai.com/gtkloqqiwc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtnhpchqxk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtafmtfmmb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtdchyexmf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtmqythsaj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.quarkkingdee.top/gtjvfmjjgy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtktgwvgke.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xziqi.cn/gtfrhhjrfm.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtafxjrnrx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtdpzzimlb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtrudvnxde.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtnivrtzjc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtkcegybte.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.daxiang520.top/gtowifnjpt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtikisgjds.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtkkertbom.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtigngggmj.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtvjblqtjp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cheryme.top/gtvtuomkkz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtzkuvvmyl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gtcpjsvwjc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtmxqaezus.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtkzdghpee.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.guannengcc.top/gtjeacltbt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yonumen.top/gtixejktev.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtgkvijywz.html

[F05] 判断文件或目录是否存在
来源：http://hz.pycfn.com/gtblswoxlj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cdnleiting.top/gtdfqberia.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtworjhjut.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtnznjwkmb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtodydtych.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtcdcqndqp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gtqvwiborb.html

Ruby: File.exist?("a.txt")
来源：http://hz.tanke756.top/gtenbenhsi.html

C#:   File.Exists("a.txt")
来源：http://hz.jianghu66.top/gtyapexbjg.html

[F06] 删除文件
来源：http://hz.havefunace.top/gtqmiugdih.html

Py:   os.remove("a.txt")
来源：http://hz.9152youxi.cn/gteksdjwen.html

PHP:  unlink("a.txt");
来源：http://hz.mhx1999.top/gtlfivcbxh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtrbajrlny.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtiykcpqot.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtnxjbbucf.html

Go:   os.Remove("a.txt")
来源：http://hz.shzxlz.cn/gthsvjjbjp.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gtmzrsnttk.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtouyvjacr.html

[F07] 创建目录（含多级）
来源：http://hz.shzxlz.cn/gttqovhhrb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtaukkmdkj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtvqecxtfl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtsxwhcvbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gttmjoihkr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtebvtjcml.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtengqzscn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtreqnrsso.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cheryme.top/gttluflzbo.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtvhiqnumy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtzvkkmcvb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.haohaochexian.top/gtqixulrmc.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtapkklnsh.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhongyouzk.top/gtobkstmpi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gttnjtatgm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydzc1.top/gtycrtnlws.html

Ruby: Dir.children("dir")
来源：http://hz.yvedp.cn/gtncmywimc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtprwxiryl.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtobwkcbnc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jlsjyb.cn/gtvaouwjsr.html

PHP:  filesize("a.txt");
来源：http://hz.quarkkingdee.top/gtvkxcztvt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtgvtqohwk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtlyylmywm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtcjfydues.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cucudq.cn/gtxtucvgrj.html

Ruby: File.size("a.txt")
来源：http://hz.chenzaomai.com/gtiddcquln.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sysykeji.top/gtydttmqhv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gttcqqdmdq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtvafrrpgr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hongshengwenyu.top/gtcstgoyxf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtmmiuwrkz.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gtrwwjwvum.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zycfv.cn/gtgxrwkvxu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtbrsjwdlq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gteczyaeek.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.mhx1999.top/gtvuignnth.html

[F11] 复制与移动文件
来源：http://hz.bjfxy.top/gttgeawgkx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtobsmpbwy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gtigwhlilv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gttudzoprh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gttvihbjde.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgfzy.top/gtykvdcrpv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtyywpdirl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtiozbvspt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtojbdokfk.html

[F12] CSV 读写
来源：http://hz.snrcjt.cn/gtjwxnstbq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.9152youxi.cn/gthmsxzucm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxinkj.top/gtzsqzesos.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtzshkunyb.html

TS:   // 同上
来源：http://hz.shuidangran.top/gtgnmmkxir.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnxiangtu.top/gtpffnswyp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gthfkaeeyv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtrtajzrae.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj202588.top/gtsjezuvmn.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqvgttbef.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtfqludhlw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdixgybgw.html

[G01] 定义类
来源：http://hz.cashguo.top/gtpbnhatyw.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtbkchssux.html

PHP:  class User {}
来源：http://hz.gzhubu.top/gtkwmcwfap.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gtmrxwoagt.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtarhjzwrz.html

Java: class User {}
来源：http://hz.daxiang520.top/gtfjgmqwiz.html

Go:   type User struct { Name string }
来源：http://hz.yvedp.cn/gtyriflhhx.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtiskrzspf.html

C#:   class User {}
来源：http://hz.daria6918.cn/gtcjcargjb.html

[G02] 构造函数
来源：http://hz.cashguo.top/gtqolbnpkn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dashuyun.cn/gtgvtabqra.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuxming.cn/gtpsdzavbg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuanzx.com/gtgohbebua.html

TS:   constructor(public name: string) {}
来源：http://hz.dianchejie.cn/gtsyyzsyvw.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtbuymgrwr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gtvhnpyjkk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtnuaszkbl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aizwys.cn/gtaljbtrqt.html

[G03] 实例属性
来源：http://hz.quarkkingdee.top/gtsuzrchhb.html

Py:   self.name = "x"
来源：http://hz.chenlongwang.top/gtpdhgrloe.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtrghrdtrm.html

JS:   this.name = "x";
来源：http://hz.birdmap.top/gtnngqgkqg.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gtdloswizs.html

Java: private String name;
来源：http://hz.redwolf501.top/gtsmutabjv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gtciapekov.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtydvhscev.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtimweilpy.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gthpcmhrxi.html

Py:   def greet(self): return self.name
来源：http://hz.yonumen.top/gtnfxlnbpw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtstrohtgl.html

JS:   greet() { return this.name; }
来源：http://hz.aibaodan.cn/gtqydgrgxr.html

TS:   greet(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtabzuwpgb.html

Java: String greet() { return name; }
来源：http://hz.tian-w.cn/gtrvflorwp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtieeajocj.html

Ruby: def greet; @name; end
来源：http://hz.aizwys.cn/gtgzufopsc.html

C#:   public string Greet() => Name;
来源：http://hz.9152youxi.cn/gtzdnjvalf.html

[G05] 继承
来源：http://hz.nanxuanxn.top/gtxkkhxwcl.html

Py:   class Admin(User): pass
来源：http://hz.ydjk.org.cn/gtzoulykag.html

PHP:  class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtasrcswnh.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtqqafdqgx.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtzifukjli.html

Java: class Admin extends User {}
来源：http://hz.xinyue.icu/gtgsdasomj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gttprovihi.html

Ruby: class Admin < User; end
来源：http://hz.jinqigufen.top/gtxldgzeyz.html

C#:   class Admin : User {}
来源：http://hz.ybcxt.top/gtfowhzmmx.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gtyxcggwxp.html

Py:   def greet(self): return "admin"
来源：http://hz.xylfe.cn/gttxhvpecs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtwnaeektw.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gthpteljzt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtaxbhpopo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gtvfgpcrvj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gtepjsnfuo.html

Ruby: def greet; "admin"; end
来源：http://hz.andypj.xyz/gtkfzxtxbk.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtymcprjay.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gthmfxffbf.html

Py:   super().greet()
来源：http://hz.yonumen.top/gttltqebds.html

PHP:  parent::greet();
来源：http://hz.gaohongyu789.top/gtecxawxuk.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtrtrygnkh.html

TS:   super.greet();
来源：http://hz.daria6918.cn/gtmgexfebt.html

Java: super.greet();
来源：http://hz.hammf.cn/gtyudcxaph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtctpysrul.html

Ruby: super
来源：http://hz.jiagoushi.top/gtzyseqzte.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtdohejduo.html

[G08] 静态方法与属性
来源：http://hz.nanxinkj.top/gtxjwvjngp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gtwgxrpvev.html

PHP:  public static function f() {}
来源：http://hz.sufxvd.cn/gthioftrvg.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtcudcqori.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtfkzgwxbe.html

Java: static void f() {}
来源：http://hz.zhiwuduotai.top/gtphjkypeu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtgyfsmqfa.html

Ruby: def self.f; end
来源：http://hz.ehwqpu.com/gtjsucmdrb.html

C#:   public static void F() {}
来源：http://hz.sweek.top/gtrmolifkt.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gtzaqcraez.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtglsyhhjk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.iojbl.cn/gtlsfdyyoj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xingfuxueyuan.xyz/gtnuzdhexf.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtjbprpijd.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtgvdgmizx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtmmpmrtpy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.bjfxy.top/gtigrvtyya.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtayyqviji.html

[G10] 访问控制
来源：http://hz.zdqjudy.top/gtdyzhgrzw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtpqxqtwva.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtpgdsqnhq.html

JS:   #private 字段；其余公开
来源：http://hz.chenjidiqi.icu/gtwjwtxxok.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtruqckrzd.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtccpjytxj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.havefunace.top/gtxzrqhqey.html

Ruby: public / protected / private
来源：http://hz.yongpay.top/gtqhsizcfk.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtwhqlvacz.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtoekizyck.html

Py:   @property 与 @x.setter
来源：http://hz.aibaodan.cn/gtpahwzdxd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtylaagrwn.html

JS:   get name() { return this._name; }
来源：http://hz.yanxiufei.cn/gtuctxgfoj.html

TS:   get name(): string { return this._name; }
来源：http://hz.aizwys.cn/gtymsotftk.html

Java: public String getName() { return name; }
来源：http://hz.zycfv.cn/gtjbknnkkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtpsbsaurr.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtqsimbfdz.html

C#:   public string Name { get; set; }
来源：http://hz.tanke756.top/gtlavcijsy.html

[G12] 对象转字符串
来源：http://hz.nanxinkj.top/gtplanqnvv.html

Py:   def __str__(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtflvahvis.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gthakyhywj.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtnwvowvoa.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtuvotdwty.html

Java: @Override public String toString() { return name; }
来源：http://hz.gaohongyu789.top/gtbmxsqonr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.smart0.xyz/gtpkeekans.html

Ruby: def to_s; @name; end
来源：http://hz.sweek.top/gtjpnfwubj.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gtsaatppka.html

[G13] 判断对象类型
来源：http://hz.jianghu66.top/gtqwbvnjky.html


<!-- 参考信息 -->