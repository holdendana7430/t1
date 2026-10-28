代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinghuilouyu.cn/gtmefpqyqn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhixingplan.top/gtazsbhgzo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtomzqsatq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258.top/gtynuhvibv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydjk.org.cn/gtllicukhx.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigufen.top/gtfzggnnpd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtdjbwimdh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtbylllbol.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xylfe.cn/gtvypzuove.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtitjdvvvi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtrjbbdnrx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.havefunace.top/gtkrmfynoj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtrqogxrlh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtrtdcvwrs.html

[E16] 数字千分位
来源：http://hz.yonumen.top/gtqvrdswar.html

Py:   f"{1234567:,}"
来源：http://hz.kuanghao11.cn/gtdtodoxky.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtmoghpftf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtelvgqwen.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtaywyedke.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.kuanghao11.cn/gtvjotgxbl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gtlnjblegn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yanxiufei.cn/gtbejwpasx.html

C#:   1234567.ToString("N0")
来源：http://hz.snrcjt.cn/gtpyqpvbzf.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtruivuuec.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtrhzcqirx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cheryme.top/gtnrftzfdf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shuidangran.top/gtejbisnrh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtqdxjawkw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtpxilbrqy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fengsongda.top/gteskxdygp.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gtphpnyxip.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtmkltmzwv.html

[E18] 模板占位符替换
来源：http://hz.jinqigufen.top/gtuunvtjwm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnxiangtu.top/gtteqbqnps.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuetiantiany.cn/gtzdpfkjgu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtqolxpshn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtkpbiprck.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sysykeji.top/gtnehrijes.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtcjwypndu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinyuanbaomall.cn/gtpxjcqgpm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.316326.xyz/gtusknbbht.html

[E19] 多行文本按行拆分
来源：http://hz.316326.xyz/gtrgyfxqsn.html

Py:   s.splitlines()
来源：http://hz.andypj.xyz/gtikychrda.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtocxykflb.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtiprqpnro.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gthoqowmph.html

Java: s.lines().toList()
来源：http://hz.yuxming.cn/gtbewyleep.html

Go:   strings.Split(s, "\n")
来源：http://hz.cqqwz.cn/gtsvnxhhsc.html

Ruby: s.lines
来源：http://hz.xinyue.icu/gtlgvkjnyx.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gtpclymmvl.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangtech.top/gtzxhkdcos.html

Py:   if not s:
来源：http://hz.cashguo.top/gtwvzchxjm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenjidiqi.icu/gtvypgivym.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtrksmtboc.html

TS:   if (s === "") {}
来源：http://hz.zhaomingkeji.xyz/gtgeeoginq.html

Java: if (s.isEmpty()) {}
来源：http://hz.gzhubu.top/gtkaizrwkk.html

Go:   if s == "" {}
来源：http://hz.hysaishi.cn/gtvcsqulvg.html

Ruby: if s.empty?
来源：http://hz.jyoumei.cn/gtnsjyluiw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gtvmrccchg.html

[E21] 超长截断加省略号
来源：http://hz.xylfe.cn/gtdmqthurq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hammf.cn/gteoeugqnc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.mhx1999.top/gteqfdtcuo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtuxjfvfde.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtxuyhgtat.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtzblayoxr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gogol.net.cn/gtewofptps.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gtaqurpkvz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shuidangran.top/gtdplpqsqn.html

[E22] 字节长度与字符长度
来源：http://hz.xuetiantiany.cn/gtxvddqyje.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtamkkjdqx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtluouytnq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gthvzkgzje.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtyjrwqwbv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhoulong.xyz/gtdkvuikgv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtdteldskk.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gttpayaklm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guannengcc.top/gtfhsprxwp.html

================================================================================
来源：http://hz.tianlin.xyz/gtesqkqccr.html

F. 文件与目录
来源：http://hz.jlsjyb.cn/gtorsybigl.html

================================================================================
来源：http://hz.guannengcc.top/gtrbgfpioe.html

[F01] 读取整个文件
来源：http://hz.xuanzx.com/gtlkysqxxn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gteheijmpn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhiwuduotai.top/gtcdtpznrm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinyuanbaomall.cn/gtphjtsomu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hfpthk.cn/gtgawksajv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtizwuczrv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangtech.top/gttvshmjkk.html

Ruby: File.read("a.txt")
来源：http://hz.xinyue.icu/gtpnbbzzae.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.0kj1m.cn/gtshuxtjiq.html

[F02] 逐行读取文件
来源：http://hz.yongpay.top/gtfazfluzr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtypypaozj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.316326.xyz/gtfpgrkdgl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtyqgslmyl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gteotayecl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtbidmnswq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.smart0.xyz/gtipfknbph.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pycfn.com/gtwcutxsfs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtjeeytuai.html

[F03] 写入文件（覆盖）
来源：http://hz.chenjidiqi.icu/gtdwmnotrj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtmxlugyup.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtbunhumbo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtfbqqyhmj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtkcmflzyj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnqzz.top/gtohbxoyjj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangkeji.top/gtxuxifpry.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhoulong.xyz/gtplfrhuch.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtflpcmptg.html

[F04] 追加写入文件
来源：http://hz.pycfn.com/gtlqbzhnqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258888.top/gtxzirirgv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtqedmvayn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtxlymxsuf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtawscvnun.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhiwuduotai.top/gtidbzyuec.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shangyingyoupin.top/gtkycjolcg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtquejkxzk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gtklxghasi.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtymrojzbf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangdashe.top/gtnmlkldmc.html

PHP:  file_exists("a.txt");
来源：http://hz.yuanzhike.top/gtzritkhjt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtcikmutvt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtjdlkgkxb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtqmwiziog.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.snrcjt.cn/gtivrutpde.html

Ruby: File.exist?("a.txt")
来源：http://hz.pengpengdd.cyou/gtagrqpvgo.html

C#:   File.Exists("a.txt")
来源：http://hz.aibaodan.cn/gtaryexpvb.html

[F06] 删除文件
来源：http://hz.jlsjyb.cn/gtdjdeonut.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtcgoujczf.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtrffdkdxd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtvnljwxgx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtprtohnsx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtaiozkzht.html

Go:   os.Remove("a.txt")
来源：http://hz.dianchejie.cn/gtmwzgainl.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtbfiqdhqc.html

C#:   File.Delete("a.txt");
来源：http://hz.bjfxy.top/gtkaqnqrsh.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtrtwseclu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtxikvremz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtdkgmeqrz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtnujymkoq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtbypreisn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gtyylqqlzf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtxavmegzm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinyuanbaomall.cn/gtacflbmok.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gtpktlscuj.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtsbfyyibv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sufxvd.cn/gtrlnucpts.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zycfv.cn/gtuotqtteb.html

JS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtzyzezopl.html

TS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtrxiefiof.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtoaxnvana.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtlsxubmwo.html

Ruby: Dir.children("dir")
来源：http://hz.haohaochexian.top/gtejygluad.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gthzkbyjlv.html

[F09] 获取文件大小
来源：http://hz.jinqigfzy.top/gtopycecsb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtbgkkbdac.html

PHP:  filesize("a.txt");
来源：http://hz.nanxinkj.top/gtoynmllqv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtiaxkertt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtnmdzqael.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtwhhxzrqb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtzphwtvhw.html

Ruby: File.size("a.txt")
来源：http://hz.zhoulong.xyz/gtlnuulbad.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtgydyygqf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtxwzctphm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtocgfgzfa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnqzz.top/gtiokrgdjm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gturtshdik.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangtech.top/gtslnheekn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gogol.net.cn/gtspbultxb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtttigroxq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtovojwqbp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cashguo.top/gtdvthqdve.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtrrkqysmz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtjtscpkip.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtcgetzxob.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gteehayqtk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtxbiqfbqg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cqqwz.cn/gtnsytauoj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtrugncewo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtmqytrpon.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtfvquzyxk.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gtouhtdsws.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtqbzaxaxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daxiang520.top/gtowbexmmq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.smart0.xyz/gtwqwhmbth.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtulzozanz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gttgblsfik.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtuuecveia.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtzukfrylr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jianghu66.top/gthtvgyydd.html

================================================================================
来源：http://hz.fzhhl.top/gtcipwecvp.html

G. 面向对象
来源：http://hz.xylfe.cn/gtzjhmlrqj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjoinqnml.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtcvkjesto.html

Py:   class User: pass
来源：http://hz.chenzaomai.com/gtzhrgesgd.html

PHP:  class User {}
来源：http://hz.haohaochexian.top/gtninohvmi.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtjnxfxbwx.html

TS:   class User { name: string = ""; }
来源：http://hz.hammf.cn/gtinlredyn.html

Java: class User {}
来源：http://hz.jinyuanbaomall.cn/gtehoxkkvt.html

Go:   type User struct { Name string }
来源：http://hz.gzhubu.top/gtaalwbmvr.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtglmssrmi.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtiibbkvjt.html

[G02] 构造函数
来源：http://hz.havefunace.top/gtgqjsvjyy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtszbyueii.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtynduowiv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtphkoexzt.html

TS:   constructor(public name: string) {}
来源：http://hz.gzhubu.top/gtwtgkwspa.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtisyeyiax.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.snrcjt.cn/gtopqojtam.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gthbrikzpq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtyexwiwni.html

[G03] 实例属性
来源：http://hz.zdqjudy.top/gtdtazycnq.html

Py:   self.name = "x"
来源：http://hz.jqgfzy.top/gtodpyjcbq.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtgsfijcvh.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtbnpokshb.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtqzbhbnyj.html

Java: private String name;
来源：http://hz.yongpay.top/gtirylvnnv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtjwgsccsd.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtkkcoqjia.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.feifeiyinyue.top/gtvnwhgojk.html

[G04] 定义方法
来源：http://hz.shzxlz.cn/gtpkgfeysn.html

Py:   def greet(self): return self.name
来源：http://hz.feifeiyinyue.top/gtydvluaar.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtlbkuwajx.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtfuiaeqni.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gtgxjfvehk.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtwlvgiuzp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtqwiowgbv.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtgqacvvja.html

C#:   public string Greet() => Name;
来源：http://hz.ehwqpu.com/gtdkybfdes.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtepytjmhl.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtofepdjks.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtscekqkvz.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtipyzcyej.html

TS:   class Admin extends User {}
来源：http://hz.ivvv.top/gtdhumgchj.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtkhxkehtk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dianchejie.cn/gtpylcaalk.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtrrtpinad.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gthpnniqnk.html

[G06] 重写方法
来源：http://hz.sysykeji.top/gtgnsfrurx.html

Py:   def greet(self): return "admin"
来源：http://hz.xinyue.icu/gtaqziggod.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtiedswoet.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtjntlnxot.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtxvsoyhsk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtcgkquxrt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtcbgoaqiv.html

Ruby: def greet; "admin"; end
来源：http://hz.birdmap.top/gtmxbqhptc.html

C#:   public override string Greet() => "admin";
来源：http://hz.tanke756.top/gtbfizxpkf.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtpikyhoyl.html

Py:   super().greet()
来源：http://hz.zdqjudy.top/gtiiywylkp.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gterufqenh.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtipwflebt.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtcdexsxlv.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtkvirmnpb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtqawelskh.html

Ruby: super
来源：http://hz.yongpay.top/gtyjpdjnla.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtddtbfnyd.html

[G08] 静态方法与属性
来源：http://hz.yanxiufei.cn/gtmqhtyzgn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtdivvfdom.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gtqlddmjny.html

JS:   static f() {}
来源：http://hz.jiagoushi.top/gtrxpdflll.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtbchiqsqz.html

Java: static void f() {}
来源：http://hz.aizwys.cn/gtgkhdjlvc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xingfuxueyuan.xyz/gttksixduk.html

Ruby: def self.f; end
来源：http://hz.sufxvd.cn/gtnwlovjqt.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtudfejknf.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtzftqjvhl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtjjbxbsvc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtgxbmrbnm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gthojjkdmg.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtibbdbjzl.html

Java: interface Shape { double area(); }
来源：http://hz.ydzc1.top/gtswyyfxsv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtdogvubii.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtgdizbwio.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtlzcuaflg.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtqdltufhk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gtttlmqdhu.html

PHP:  public / protected / private
来源：http://hz.quarkkingdee.top/gtgzfulbql.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtdzinhita.html

TS:   public / protected / private
来源：http://hz.yonumen.top/gtwjkcyqjx.html

Java: public / protected / private / 默认包级
来源：http://hz.fzhhl.top/gtyzwdnugl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtojtuxffg.html

Ruby: public / protected / private
来源：http://hz.yuanzhike.top/gthzawridu.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtiadbqxum.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtfvwuyrty.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gtiucubsyu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtewgnatpl.html

JS:   get name() { return this._name; }
来源：http://hz.c1oappe.top/gtagfekrbx.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnxiangtu.top/gtyiqvywtd.html

Java: public String getName() { return name; }
来源：http://hz.zhiwuduotai.top/gtglkygced.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtkipuxxzr.html

Ruby: attr_accessor :name
来源：http://hz.pengpengdd.cyou/gtawpjyuus.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gtdmhvwwqu.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtvhpxcmbi.html

Py:   def __str__(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtdwgqabza.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gtpxjvjfwo.html

JS:   toString() { return this.name; }
来源：http://hz.smart0.xyz/gttcjxtqbx.html

TS:   toString(): string { return this.name; }
来源：http://hz.yvedp.cn/gtkibwtbjl.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhijiandao.cn/gtcdxmordw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ybcxt.top/gtgswvnquh.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtfdpjbhjf.html

C#:   public override string ToString() => Name;
来源：http://hz.gogol.net.cn/gtvcqycqqm.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtqbiehftp.html


<!-- 参考信息 -->