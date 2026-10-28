代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgfzy.top/gtqbhfmxwi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtirggjmxl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dianchejie.cn/gtddkuvyki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtukrxraqq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gtmsdwlomc.html

[E15] HTML 转义 / 反转义
来源：http://hz.cheryme.top/gtupjtronb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yvedp.cn/gtpigydnkn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.kuanghao11.cn/gtzlnwuewy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtoyktbttb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtmbzdwuxa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.smart0.xyz/gtzpsgkxty.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tian-w.cn/gtwbdvlfhv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgfzy.top/gtklmztosk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gthiaklycf.html

[E16] 数字千分位
来源：http://hz.birdmap.top/gtkfdbwfbh.html

Py:   f"{1234567:,}"
来源：http://hz.xuetiantiany.cn/gtzisgzyhg.html

PHP:  number_format(1234567);
来源：http://hz.c1oappe.top/gtkojkdyvy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gtnmerfxiw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtjnznwjhj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cdnleiting.top/gtsjqxfqtj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtnacsajyo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.fengsongda.top/gtzldmsxcs.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtzfeflpyd.html

[E17] 首字母大写
来源：http://hz.cashguo.top/gtyeysvrov.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cucudq.cn/gtskhcwtfw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yvedp.cn/gtzwtozmbb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtrthkrcuo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gthzlhgked.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nwbrower.top/gtwkvcxion.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtyxpqwbtg.html

Ruby: s.capitalize
来源：http://hz.hysaishi.cn/gtvnfjpqia.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhijiandao.cn/gtvlpnqvyi.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtoojtnttc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj202588.top/gtelywbeoa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.kuanghao11.cn/gtkcirlmqh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtmjpdohxv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtnqeirsfi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gtkzwrvvqa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtlsqdjuaz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shzxlz.cn/gtooqzfdvi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sxryk.cn/gtwzhsxvlh.html

[E19] 多行文本按行拆分
来源：http://hz.chenzaomai.com/gtxskjsfet.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtzemwibvt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gtjwdsvgbr.html

JS:   s.split(/\r?\n/)
来源：http://hz.jiagoushi.top/gtkuejjirr.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtnqdwbtfz.html

Java: s.lines().toList()
来源：http://hz.feifeiyinyue.top/gtpqyyxqfk.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtohmplwpv.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtcljwrvbr.html

C#:   s.Split('\n')
来源：http://hz.yj202588.top/gtfquluuyu.html

[E20] 判断字符串是否为空
来源：http://hz.pycfn.com/gtfimhokhc.html

Py:   if not s:
来源：http://hz.yanxiufei.cn/gtmjalbhzs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sysykeji.top/gtesltwwgw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtksswwmqz.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtrqctuqdv.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigufen.top/gtnszahyvq.html

Go:   if s == "" {}
来源：http://hz.vqdsnc.cn/gtaxzczczu.html

Ruby: if s.empty?
来源：http://hz.aibaodan.cn/gtlthrlbyx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ywan-chungtsiang.top/gthdojpcbp.html

[E21] 超长截断加省略号
来源：http://hz.316326.xyz/gtftqjatvz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yonumen.top/gtnanenedc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shangyingyoupin.top/gtnhfipauv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gthsqigdth.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtllurqgka.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtqvxptuvp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pengpengdd.cyou/gthexrdnuo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtnaidwhez.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dashuyun.cn/gtrmmrvzqk.html

[E22] 字节长度与字符长度
来源：http://hz.zdqjudy.top/gtjrhhnwdm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ybcxt.top/gtumottjnl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtevgjelyi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtjhgdemmm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gtnpverjpx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dianchejie.cn/gtebkcdsrc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sxryk.cn/gtbhkxewwx.html

Ruby: s.bytesize;  s.length
来源：http://hz.ehwqpu.com/gtqyvcdhag.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtduiprsyo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxzdvbuak.html

F. 文件与目录
来源：http://hz.cucudq.cn/gttnaokldu.html

================================================================================
来源：http://hz.nwbrower.top/gtmrebwaei.html

[F01] 读取整个文件
来源：http://hz.yonumen.top/gtjdnhqymx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sufxvd.cn/gtzakflzfc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtyfeuwhel.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtbbmcwkvg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgfzy.top/gthqgdpyxe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtuurlasrh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtgjaegnqj.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtgljpulfg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtjdufmgna.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gtscwkowkz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhoulong.xyz/gtjwwdjgde.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gtbmeyyzxn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gttfnffysa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtvaojntod.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtgwtpqfuz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtiqgbgcvx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenjidiqi.icu/gtjdvvopuh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtumfbphhh.html

[F03] 写入文件（覆盖）
来源：http://hz.yonumen.top/gtcdobukqj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cqqwz.cn/gtcjuztpja.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtfgbhvnzb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtxchybswf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtuifcuczh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shangyingyoupin.top/gtqmtagexc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pengpengdd.cyou/gtzxurnagh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.bjfxy.top/gtdkzgpage.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtogetwofl.html

[F04] 追加写入文件
来源：http://hz.chenlongwang.top/gtrjquwtwr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtbgrqzjyk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtqwkayhdw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cucudq.cn/gtnrszattz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtoawjilee.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shzxlz.cn/gtlywtfjry.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.svipenyu.cn/gtdfldpipv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhongyouzk.top/gtgjtgcroa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtngvbdgqe.html

[F05] 判断文件或目录是否存在
来源：http://hz.xinyue.icu/gtomjfmwjp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sweek.top/gtgvotgtvt.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtvbhdwbob.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtsrydlzax.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtzqffnyej.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtjplbkgpa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.c1oappe.top/gtqcfbkrtj.html

Ruby: File.exist?("a.txt")
来源：http://hz.tianlin.xyz/gtbspynyoo.html

C#:   File.Exists("a.txt")
来源：http://hz.iojbl.cn/gtjjuvyvrn.html

[F06] 删除文件
来源：http://hz.andypj.xyz/gtipirklpu.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtdowjfary.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtbgjzopoa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daxiang520.top/gtklxnwivi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gtglgitcsv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gthxabetiy.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtgbigekrw.html

Ruby: File.delete("a.txt")
来源：http://hz.cqqwz.cn/gttwnygshp.html

C#:   File.Delete("a.txt");
来源：http://hz.jlsjyb.cn/gtsxkxhogq.html

[F07] 创建目录（含多级）
来源：http://hz.yonumen.top/gtckxbuvgx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtqtlqocoq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gttnrhurqb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtfolbkkgf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gthuihizvf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhijiandao.cn/gtpfoagdpj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtzgwcblmq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pengpengdd.cyou/gtjcdlkxts.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ehwqpu.com/gtfwzjatkq.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gtbuhrvpog.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtnnwbtecr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yangfankeji.com/gtlrsxyexo.html

JS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtqyclfsww.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtegzfpcmk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtwoqvhjyg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gtecalmggv.html

Ruby: Dir.children("dir")
来源：http://hz.redwolf501.top/gtpvpmknhj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtfyxalmmf.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gteowgqyva.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tanke756.top/gtpddlntmx.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtwzvtkhpl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtpkaaltdc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gtkhlsfulr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtuaqkmcxz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtchmsaoso.html

Ruby: File.size("a.txt")
来源：http://hz.dianchejie.cn/gtqhayxdzt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gthiwqxsnj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gtncxetczp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtdhoyoibz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aizwys.cn/gtzqkjutcc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtmsxeqqfp.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtudzlrqrj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gteftftfgb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtwykfddij.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtlcuptlpf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtnaciyhwy.html

[F11] 复制与移动文件
来源：http://hz.sweek.top/gtemhajdxb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtflioqotx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sweek.top/gtxocexezl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtvalgwqhw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtrqwuisec.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.mhx1999.top/gtuxsqldam.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj202588.top/gtnerxrhgo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtyrbcruvr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yangfankeji.com/gtqtrpupmy.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtwoxiaxnf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.birdmap.top/gtgadcrhat.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnxiangtu.top/gtgvhkkdyy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhongyouzk.top/gtjwylpivd.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gttuuhhwlh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtgidyjalf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtbhsgkkzx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guannengcc.top/gtfwwqixvo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.mhx1999.top/gtbmkgbrhv.html

================================================================================
来源：http://hz.ehwqpu.com/gtohkexxuc.html

G. 面向对象
来源：http://hz.wangdashe.top/gtsbiacyxj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtcynqtfyw.html

[G01] 定义类
来源：http://hz.yanxiufei.cn/gtabzxpciv.html

Py:   class User: pass
来源：http://hz.sufxvd.cn/gtsryjbnyf.html

PHP:  class User {}
来源：http://hz.jqgufenzy.top/gtymhrxvah.html

JS:   class User {}
来源：http://hz.mhx1999.top/gttghqbbjm.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtmidyetzg.html

Java: class User {}
来源：http://hz.cashguo.top/gtiboerttm.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtgzcmqtmd.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gtmbtzlgds.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtyukqoknh.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtwqoanpoy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtrclxrjtc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gttgysivoo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gttwmznyqh.html

TS:   constructor(public name: string) {}
来源：http://hz.pycfn.com/gtqqczofhr.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtxmwvtroi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtcfwzcaok.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtekynnetx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtpzqcnbou.html

[G03] 实例属性
来源：http://hz.meibo888.top/gtsvlkibbm.html

Py:   self.name = "x"
来源：http://hz.yueranfly.top/gtmuopucyd.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gtcmhyjtqj.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtzodkygyc.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtjrrvwjbj.html

Java: private String name;
来源：http://hz.svipenyu.cn/gtosuejcqb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gtvnjeagfm.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtevrdxdvz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtlumtwnfi.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtxmgyzjbj.html

Py:   def greet(self): return self.name
来源：http://hz.kuanghao11.cn/gtiugmsgnf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtiyradnzc.html

JS:   greet() { return this.name; }
来源：http://hz.tian-w.cn/gtbkynzcbw.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigufen.top/gtwzlyzfkw.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtckigyeyb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aibaodan.cn/gtntrkaoap.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtlnrnvwtg.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtcpultyxw.html

[G05] 继承
来源：http://hz.hywenlv.cn/gtlyhseiam.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtlviycuip.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtwhzmichp.html

JS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtmcldwcdu.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtuazwdogf.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtaukcxbhg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtkijoqetu.html

Ruby: class Admin < User; end
来源：http://hz.dashuyun.cn/gtiolplnnx.html

C#:   class Admin : User {}
来源：http://hz.tanke756.top/gtnuyifpyf.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtpsjqadym.html

Py:   def greet(self): return "admin"
来源：http://hz.ywan-chungtsiang.top/gtegozsjdz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtzdaxoija.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258.top/gtjqvgxncq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtetchmjvy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtzrorwcwe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtesmfrchz.html

Ruby: def greet; "admin"; end
来源：http://hz.ybcxt.top/gtkmvbbjiz.html

C#:   public override string Greet() => "admin";
来源：http://hz.ybcxt.top/gtvcagkogj.html

[G07] 调用父类方法
来源：http://hz.snrcjt.cn/gtejdcnucg.html

Py:   super().greet()
来源：http://hz.chenzaomai.com/gtyddvdviw.html

PHP:  parent::greet();
来源：http://hz.sweek.top/gtvnzjiwzh.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtuemmnxss.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtpivzdywd.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gtyhnehoay.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ybcxt.top/gtswflhcxh.html

Ruby: super
来源：http://hz.ybcxt.top/gtcaskwqkt.html

C#:   base.Greet();
来源：http://hz.ppjwa.cn/gtmryihkyn.html

[G08] 静态方法与属性
来源：http://hz.cheryme.top/gtepfcvhgd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhoulong.xyz/gtjgzjqqde.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtmlkzqlmx.html

JS:   static f() {}
来源：http://hz.yj20258888.top/gtfoxjbkgx.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtibuwyasq.html

Java: static void f() {}
来源：http://hz.jqgufenzy.top/gtzrswowmk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gtcwdrwhfz.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gthnichhyf.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gtdqjvlhol.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtmxggpvop.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtgwjzizgf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtaabbcfol.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenjidiqi.icu/gtfuqqryib.html

TS:   interface Shape { area(): number; }
来源：http://hz.hongshengwenyu.top/gtyrmugoqw.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gttiwlrjva.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtadvbvihz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgfzy.top/gtrlvujznj.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtabdsvizw.html

[G10] 访问控制
来源：http://hz.cqqwz.cn/gtkghtrunj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guowangkeji.top/gtovrektmb.html

PHP:  public / protected / private
来源：http://hz.xuetiantiany.cn/gtyjhkospj.html

JS:   #private 字段；其余公开
来源：http://hz.nanxuanxn.top/gtcxwudpyv.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gthnpzbokx.html

Java: public / protected / private / 默认包级
来源：http://hz.tian-w.cn/gtwcrzpxld.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtrqgwmoqx.html

Ruby: public / protected / private
来源：http://hz.gaohongyu789.top/gtmbklzvcv.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtivdxedpx.html

[G11] getter / setter
来源：http://hz.hongshengwenyu.top/gtmrqrmwfz.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtirsqjqui.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtxtztfhdb.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gtoizcwutq.html

TS:   get name(): string { return this._name; }
来源：http://hz.nwbrower.top/gtbtliapyp.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtjmfepipv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hfpthk.cn/gtmkkpakvn.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtwhdrwigm.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtawiisxmy.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gterrwausf.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtjlrhgcmb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtlqwyeobt.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtqhrpagpj.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtzsiiiwob.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtsycrepyj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtnsdsocpn.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtijsydpoo.html

C#:   public override string ToString() => Name;
来源：http://hz.jlsjyb.cn/gtbrdscvhg.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtmsjtkeyp.html


<!-- 参考信息 -->