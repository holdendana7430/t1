代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gtsofwmyui.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtijpglxat.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cashguo.top/gtxrjysajl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gthbctgvwn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydzc1.top/gtxhlvqfnk.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinyuanbaomall.cn/gtdbiviwau.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shzxlz.cn/gtuqpaodnu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hfpthk.cn/gtgiuxznqn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenjidiqi.icu/gtexqkhesx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cheryme.top/gtcvlnpgmz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ppjwa.cn/gtdstofwcz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hfpthk.cn/gtwhofkhbc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.redwolf501.top/gtlercbltb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fengsongda.top/gtkursfece.html

[E16] 数字千分位
来源：http://hz.smart0.xyz/gtftfnptqf.html

Py:   f"{1234567:,}"
来源：http://hz.xingfuxueyuan.xyz/gtnyvuszrt.html

PHP:  number_format(1234567);
来源：http://hz.zhijiandao.cn/gtduyqsvjm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gthherkplb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtsygqdemc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtbvzexxxe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhongyouzk.top/gtzejwyzfb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuxming.cn/gtapofzexs.html

C#:   1234567.ToString("N0")
来源：http://hz.mhx1999.top/gtzdnfhffx.html

[E17] 首字母大写
来源：http://hz.hnqzz.top/gtepjbufgo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shangyingyoupin.top/gtskojghsw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtebnldlgc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtxrckljgg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtnmofxxjg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtvxwoppmp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gtxnuxavye.html

Ruby: s.capitalize
来源：http://hz.sysykeji.top/gtwvmgahpz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gogol.net.cn/gtralosvzr.html

[E18] 模板占位符替换
来源：http://hz.sufxvd.cn/gtzwpkbqbd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cheryme.top/gtgibqxuyv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gthqpupxey.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtxnslxjrm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtfrzzrkmm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yangfankeji.com/gthitnfscb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.haohaochexian.top/gtrqivjdto.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zycfv.cn/gtfhrcttrg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtoiigytuu.html

[E19] 多行文本按行拆分
来源：http://hz.sysykeji.top/gtijgwmzad.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtrqfoystz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtteyrvdot.html

JS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtlemhtcmp.html

TS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtlcqjoros.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gtuaebrhxv.html

Go:   strings.Split(s, "\n")
来源：http://hz.yangfankeji.com/gtnqwrhpgj.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtksvtycxy.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtukbifztk.html

[E20] 判断字符串是否为空
来源：http://hz.yuanzhike.top/gtixigutxl.html

Py:   if not s:
来源：http://hz.yuxming.cn/gtkbkrgckq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sufxvd.cn/gtqrypuerc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.redwolf501.top/gtrmaogwaw.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gtmkggwgve.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtcehhubwd.html

Go:   if s == "" {}
来源：http://hz.jlsjyb.cn/gtfewomwui.html

Ruby: if s.empty?
来源：http://hz.shzxlz.cn/gtprwvmlkg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gtvjdortno.html

[E21] 超长截断加省略号
来源：http://hz.sxryk.cn/gtxnmdfpip.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xylfe.cn/gtfjnvhxab.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.meibo888.top/gtranqwwqg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtyhciyjad.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtqugxasam.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtonuylmpf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxinkj.top/gtmuehhbly.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gzhubu.top/gtizyjzehb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtleqezbxm.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gttcojqhlw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangtech.top/gteohdqzzw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtflfybzig.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtitkuawvn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gttipyrxjp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gtiogducam.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtrhingxgt.html

Ruby: s.bytesize;  s.length
来源：http://hz.shzxlz.cn/gtgdutqifp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtkpqxmfgo.html

================================================================================
来源：http://hz.pycfn.com/gtxjcmkzxx.html

F. 文件与目录
来源：http://hz.sxryk.cn/gtqawjqsxf.html

================================================================================
来源：http://hz.xinyue.icu/gtfkzwbjsy.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gtbgxfxhii.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinqigufen.top/gtgpvptovm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guannengcc.top/gtqrcanwsh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ywan-chungtsiang.top/gtyillhxtv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.iojbl.cn/gttcexwtst.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtvxqfcked.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hongshengwenyu.top/gtldmnlgdl.html

Ruby: File.read("a.txt")
来源：http://hz.daria6918.cn/gtbwiytwmv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydzc1.top/gtndeqxeek.html

[F02] 逐行读取文件
来源：http://hz.cheryme.top/gtfsggtqbv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gttsnmojuf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gthkdumxnc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangdashe.top/gtpfywbzgd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtqebzsaba.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtvqayorck.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtvhmpuelc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jianghu66.top/gturlkulot.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhijiandao.cn/gtcvqrqnwr.html

[F03] 写入文件（覆盖）
来源：http://hz.zdqjudy.top/gtcgqzvhuf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hysaishi.cn/gtnoifufkc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtksavszjb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gttgcxodvx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtymjvbcrk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gtplgvpmgg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yuanzhike.top/gtbxgdsfbu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.316326.xyz/gttdamqtdt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtnbekmrjh.html

[F04] 追加写入文件
来源：http://hz.tianlin.xyz/gtwyzblqup.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtknazxzbe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aizwys.cn/gthszrztqg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtmowlubyp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtmtnyyzkv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhongyouzk.top/gtyiojrnwe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shangyingyoupin.top/gtujzutjsf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtfjxdemss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtwugaprsx.html

[F05] 判断文件或目录是否存在
来源：http://hz.cqqwz.cn/gtntvpayof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pycfn.com/gttxbzvxbi.html

PHP:  file_exists("a.txt");
来源：http://hz.guannengcc.top/gtroiehgzi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtisvivsib.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtdibzzvga.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtymnrtyaj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gtrvzwpnvj.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtlfxvdkqs.html

C#:   File.Exists("a.txt")
来源：http://hz.shuidangran.top/gticvsyhjt.html

[F06] 删除文件
来源：http://hz.xuanzx.com/gtjhckabcr.html

Py:   os.remove("a.txt")
来源：http://hz.tian-w.cn/gtyhgwqilh.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtvgoomkyv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtxjuqcvub.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtirqhaoss.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtfrbrdool.html

Go:   os.Remove("a.txt")
来源：http://hz.c1oappe.top/gtrtzoxdwx.html

Ruby: File.delete("a.txt")
来源：http://hz.zhengqikj.top/gtztbdwdae.html

C#:   File.Delete("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtpjrcmtsa.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258.top/gtofkwticn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtnldiidws.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtsrndntlw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtztevguvm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtuwhfiygv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhaomingkeji.xyz/gtguwdnvyn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cashguo.top/gtvnxbhenl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.birdmap.top/gtycpqtptu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhongyouzk.top/gtyexqoxxm.html

[F08] 遍历目录
来源：http://hz.zhiwuduotai.top/gtmdrvftle.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigfzy.top/gtmgzfxspr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sufxvd.cn/gtqswuuylg.html

JS:   fs.readdirSync("dir")
来源：http://hz.xziqi.cn/gtywkibukk.html

TS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtyppzluda.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gthlaewesx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenzaomai.com/gtbazplzps.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtdyblxjqd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.mhx1999.top/gttxsokbcx.html

[F09] 获取文件大小
来源：http://hz.9152youxi.cn/gtkficzbqu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtksmugtlz.html

PHP:  filesize("a.txt");
来源：http://hz.nanxinkj.top/gtmixdcmse.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtihtmntdh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtpgjzsaek.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtpsayqorm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenzaomai.com/gtxxghpbzp.html

Ruby: File.size("a.txt")
来源：http://hz.fzhhl.top/gtpntyugxv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cucudq.cn/gtkevytrqz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtcarnvgnx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtcsskzjki.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tanke756.top/gtowzokavl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtyjselidz.html

TS:   path.extname("a.txt")
来源：http://hz.yueranfly.top/gtvtzmceze.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.meibo888.top/gtmylfanll.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gaohongyu789.top/gttzmpqxpv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtavwpdvph.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtxzytjvfk.html

[F11] 复制与移动文件
来源：http://hz.xylfe.cn/gtmxuiqljr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtasvqkvsq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yuanzhike.top/gtqcvtauej.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtvmtxyvyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtzrhrespf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nwbrower.top/gtjrzeafcy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenjidiqi.icu/gtqufwkikv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtljbjiltl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.smart0.xyz/gtvhodqqls.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gtrjanwkcd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yanxiufei.cn/gtfrbykvlf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yueranfly.top/gtgepfmqrv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.vqdsnc.cn/gtkeexnqat.html

TS:   // 同上
来源：http://hz.guowangkeji.top/gtfcbuqzaz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gtyrtjaeeh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.svipenyu.cn/gtkhyfsukt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hongshengwenyu.top/gtulcduccb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hnqzz.top/gtdmdluthq.html

================================================================================
来源：http://hz.daria6918.cn/gthrvqhmkb.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtmyoyubux.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdwqrxrpm.html

[G01] 定义类
来源：http://hz.chenzaomai.com/gttmjlwujx.html

Py:   class User: pass
来源：http://hz.fzhhl.top/gtfkxircqh.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtcbgzuymd.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtockeruja.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtyjmthnpu.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtalapnkqo.html

Go:   type User struct { Name string }
来源：http://hz.jlsjyb.cn/gtbxjyqzkq.html

Ruby: class User; end
来源：http://hz.yuanzhike.top/gtjnviiowm.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtnwivlqeo.html

[G02] 构造函数
来源：http://hz.xziqi.cn/gtdavnzeet.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtypjwquzd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.feifeiyinyue.top/gtfijuprwu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtnkiptpyt.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtcseqpscx.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtstkvgjam.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cheryme.top/gtfiqgwigs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gzhubu.top/gtruecrdxc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnxiangtu.top/gtjenfxprm.html

[G03] 实例属性
来源：http://hz.fzhhl.top/gtvvdlwvkv.html

Py:   self.name = "x"
来源：http://hz.yuanzhike.top/gtffbdlsku.html

PHP:  public string $name = "x";
来源：http://hz.gzhubu.top/gtmvtlfjrk.html

JS:   this.name = "x";
来源：http://hz.aibaodan.cn/gtfsufzqws.html

TS:   name: string = "x";
来源：http://hz.nanxuanxn.top/gttqlzpzby.html

Java: private String name;
来源：http://hz.ivvv.top/gtkkeooqcg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guowangkeji.top/gtbkapvmsh.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtratboqvq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pycfn.com/gtndmwevjx.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gttezzwnmn.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtjjxuvhva.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtngnndacj.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtmarblftn.html

TS:   greet(): string { return this.name; }
来源：http://hz.52xcode.cn/gtommpmmer.html

Java: String greet() { return name; }
来源：http://hz.xuanzx.com/gtlmipskok.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydzc1.top/gtoutumaiw.html

Ruby: def greet; @name; end
来源：http://hz.gzhubu.top/gteznpuokv.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gttujaedlq.html

[G05] 继承
来源：http://hz.havefunace.top/gtvrhxhwwd.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtshltquqc.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtopdlotix.html

JS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtkymknlle.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtoqqbgmyx.html

Java: class Admin extends User {}
来源：http://hz.hammf.cn/gtcsoxvuza.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daria6918.cn/gtbjeezinx.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtagsqpfpb.html

C#:   class Admin : User {}
来源：http://hz.vqdsnc.cn/gtwojkhvyb.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtziucrwnf.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtqusuypow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtefbgeehk.html

JS:   greet() { return "admin"; }
来源：http://hz.yangfankeji.com/gthyyhhvem.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtrtyxsyki.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtbkujvklu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gthahphcwj.html

Ruby: def greet; "admin"; end
来源：http://hz.svipenyu.cn/gtxryybqwp.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gtatgtnxbv.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtglqiiovz.html

Py:   super().greet()
来源：http://hz.shangyingyoupin.top/gtumaqlvrs.html

PHP:  parent::greet();
来源：http://hz.shzxlz.cn/gticfisxul.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtfcvbjuzt.html

TS:   super.greet();
来源：http://hz.meibo888.top/gtnepoopfu.html

Java: super.greet();
来源：http://hz.meibo888.top/gtplngjkyk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtaewkumaq.html

Ruby: super
来源：http://hz.yvedp.cn/gtjhgkpevp.html

C#:   base.Greet();
来源：http://hz.pycfn.com/gtkgdyagif.html

[G08] 静态方法与属性
来源：http://hz.daria6918.cn/gtzhvalrsw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtjlzuczob.html

PHP:  public static function f() {}
来源：http://hz.jqgfzy.top/gtrprebnqz.html

JS:   static f() {}
来源：http://hz.xinyue.icu/gtjqklxsov.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtirlukzxh.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtkuuvebgg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtfjfswspm.html

Ruby: def self.f; end
来源：http://hz.feifeiyinyue.top/gtimnvdtst.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtakcfqsmj.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtqcsjlsij.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.svipenyu.cn/gtzujbrcky.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gtiqxkjxyg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gtotdrvboa.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtfpdquorf.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtxelkbahe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cashguo.top/gtpgxvibsn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ywan-chungtsiang.top/gtfssbqibp.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtnbxtknws.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtvoedoqbe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydjk.org.cn/gtvhrgzfdy.html

PHP:  public / protected / private
来源：http://hz.cdnleiting.top/gtatpfuiis.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtyhpafpnm.html

TS:   public / protected / private
来源：http://hz.ehwqpu.com/gtfmiyitpw.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtctrzsdbu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtxjrlegxp.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gtdtklpbkb.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtvgbgxdrw.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtwlyxskgu.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gtmfnplohl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtjgbnfxjh.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtcwsriyai.html

TS:   get name(): string { return this._name; }
来源：http://hz.cheryme.top/gtmkhzbesv.html

Java: public String getName() { return name; }
来源：http://hz.yvedp.cn/gtohmkyxka.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.snrcjt.cn/gttvvnpppx.html

Ruby: attr_accessor :name
来源：http://hz.hnqzz.top/gtcsepwjuh.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtfsjlrwdm.html

[G12] 对象转字符串
来源：http://hz.9152youxi.cn/gtumaednyz.html

Py:   def __str__(self): return self.name
来源：http://hz.guannengcc.top/gtikwdgwqe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtaeusxcbg.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtschqhxvl.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtqjhjsnnx.html

Java: @Override public String toString() { return name; }
来源：http://hz.pycfn.com/gththvkhqd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtxwosjtym.html

Ruby: def to_s; @name; end
来源：http://hz.pengpengdd.cyou/gtabegqrqy.html

C#:   public override string ToString() => Name;
来源：http://hz.yongpay.top/gtacuszvxo.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtvbwlgzoe.html


<!-- 参考信息 -->