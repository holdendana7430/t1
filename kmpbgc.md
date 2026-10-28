代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtaxretsbr.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtoqsyhesv.html

TS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtggjgilbj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtrphunvfw.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtabfvawju.html

Ruby: s.count("a")
来源：http://hz.yuxming.cn/gtavwvneoi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.fengsongda.top/gtpjmorczx.html

[E13] 逐字符遍历
来源：http://hz.ehwqpu.com/gtsncfkqwq.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258888.top/gtsrpwqexl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cucudq.cn/gtgqobajrm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtindpisuq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtbbujtlse.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cqqwz.cn/gtdacvbezh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnqzz.top/gtkoywdlxf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gthqfjwpjg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtazshnwyn.html

[E14] URL 编码与 Base64
来源：http://hz.zhoulong.xyz/gtcirdepso.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.meibo888.top/gthhljrfem.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtdktkcbxj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gtuykgqced.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtuiiigjbz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sufxvd.cn/gtgqyinhbs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtcdmhgouk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtaxdbeugs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cqqwz.cn/gtvhaotsmo.html

[E15] HTML 转义 / 反转义
来源：http://hz.mhx1999.top/gtjkikmjki.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj20258.top/gtqnnpozns.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sufxvd.cn/gtdytanhvo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.meibo888.top/gtyaishcgp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yueranfly.top/gtghoychda.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtygecvgrc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hfpthk.cn/gthunvvyae.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gtdijvwhft.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gtfhnidzzx.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gtgblkbqlq.html

Py:   f"{1234567:,}"
来源：http://hz.shzxlz.cn/gtydermmsm.html

PHP:  number_format(1234567);
来源：http://hz.ybcxt.top/gtfgzmoaxo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtaadtimay.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtrzpgcrqg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenlongwang.top/gtjxftiimk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.bjfxy.top/gtmvaryozs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tian-w.cn/gtlicgbwvm.html

C#:   1234567.ToString("N0")
来源：http://hz.sufxvd.cn/gtoqruqenv.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gtcahsxwij.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gtocxjvkph.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhoulong.xyz/gtmisivsub.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtkcunuily.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtpprbwpcc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtrrlratcd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxuanxn.top/gtdwfbyzle.html

Ruby: s.capitalize
来源：http://hz.iojbl.cn/gtuueceyis.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.quarkkingdee.top/gtyaifhstb.html

[E18] 模板占位符替换
来源：http://hz.fzhhl.top/gtlmbilctv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtgtuslqqn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.feifeiyinyue.top/gtwtdhlfhy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtrjorrlgn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gthclvoffn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.aizwys.cn/gtgqyayjlx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nwbrower.top/gtfbhvnohm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtdzkofmpe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnqzz.top/gtqlxonexw.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtjzeqjzvj.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtudiuenyc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtdqxdfemc.html

JS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtqtzfhfvx.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtryjdfqtb.html

Java: s.lines().toList()
来源：http://hz.c1oappe.top/gtdxmfrvnk.html

Go:   strings.Split(s, "\n")
来源：http://hz.redwolf501.top/gtviehcnyu.html

Ruby: s.lines
来源：http://hz.jlsjyb.cn/gtiauwfjrd.html

C#:   s.Split('\n')
来源：http://hz.tianlin.xyz/gtmolviqhi.html

[E20] 判断字符串是否为空
来源：http://hz.yuanzhike.top/gtrvezmcaz.html

Py:   if not s:
来源：http://hz.zdqjudy.top/gtezeixrip.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtpjxhnilj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtjddeqwiw.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtrwqyqauw.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtluljvlpz.html

Go:   if s == "" {}
来源：http://hz.cheryme.top/gtdhbygzpv.html

Ruby: if s.empty?
来源：http://hz.svipenyu.cn/gtlmswojtm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guannengcc.top/gtwrnnppxy.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtznhwbbyx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cheryme.top/gttqfctpnh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xylfe.cn/gtwuapfjoj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtigemtumn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtzzepnojt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtadykthkx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtlsgjjpyo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gtcuswcwul.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gtosotcjnx.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtxgakvvjt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shzxlz.cn/gtwryzkpss.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtsulujgdy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gttgtpkthu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtsrnioije.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtkvjycxip.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gtajoltscl.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtnbrkydpe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hnxiangtu.top/gtatuvmjxp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtvigjgyge.html

F. 文件与目录
来源：http://hz.hongshengwenyu.top/gtebahykee.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmnrmhnah.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtjzrgxcxg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gtzruxvvfy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.svipenyu.cn/gtuowlauuh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtrpxqfgqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gtnqlhnhlj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtahqrttcp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtohginjla.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtmexnpafx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hammf.cn/gtqqrftxtb.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gtlnfrwxdt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtfwefdvwf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yongpay.top/gtiefjcgye.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtwmuflvbx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gtozagvfjf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtcoktqufq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtqzzngoox.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.aizwys.cn/gtskpnpmyq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cqqwz.cn/gtnywollfy.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtjdiitjjq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgufenzy.top/gtdwltzmse.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtebttkgat.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtclohvamo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daxiang520.top/gtpbkmkynl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.smart0.xyz/gtbdgnwken.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtbgcvtbiy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aizwys.cn/gttowbnnca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtawdtldti.html

[F04] 追加写入文件
来源：http://hz.jqgfzy.top/gtxwmwtjek.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gtdjkgwtqu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cdnleiting.top/gtqwliytnp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gthmlewnww.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtlgehgilw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tianlin.xyz/gtlusuwbaa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cqqwz.cn/gtkyfftuqx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtxeovkwca.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.havefunace.top/gtdmtjryqi.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtbfcwlfxk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtsohpzfyr.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtftjjfcim.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtnqbrgvay.html

TS:   fs.existsSync("a.txt")
来源：http://hz.svipenyu.cn/gtefkweyrk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtljaxfjdd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sufxvd.cn/gtgyrzgsrh.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnxiangtu.top/gtvkvbvarh.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gturpqtdsa.html

[F06] 删除文件
来源：http://hz.zhiwuduotai.top/gtzcmsscha.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtrbhipzbe.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtktvzffia.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtezrgslud.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtlsakhwcv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtyzlnbjxv.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtrvgihjjm.html

Ruby: File.delete("a.txt")
来源：http://hz.zhoulong.xyz/gtunmujtcx.html

C#:   File.Delete("a.txt");
来源：http://hz.gotoacloud.top/gtnzmrvvxk.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtgszpmysh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aibaodan.cn/gtnwbrwsxk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.kuanghao11.cn/gtcetydawf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gttjszngfe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtbpohlbby.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sysykeji.top/gtehddfynn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtmhtrhulb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtrrkbzpyb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhixingplan.top/gtyqezcdcw.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtxteqzlle.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtrrphkbwh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yanxiufei.cn/gtypjglsrs.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtyjllduwk.html

TS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtugbcmxcj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtxfjwzefn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hammf.cn/gtphvcwwli.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtyhukiykm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jiagoushi.top/gtazxzbqga.html

[F09] 获取文件大小
来源：http://hz.jinyuanbaomall.cn/gtuxaomora.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtghjlbnit.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtnwnahhzh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtafxfzcqd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtpdygdefv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtzgdmfgha.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tanke756.top/gtdqdneblw.html

Ruby: File.size("a.txt")
来源：http://hz.0kj1m.cn/gtqcelgkvn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtlgvgaape.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnqzz.top/gtjxzhubzg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtarftwoqd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhengqikj.top/gtmxaeblah.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtdzuyxvmk.html

TS:   path.extname("a.txt")
来源：http://hz.sysykeji.top/gtjdaarciq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shangyingyoupin.top/gtcybhommh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tianlin.xyz/gtsppefleg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtwvwjsixc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gtqujefpmd.html

[F11] 复制与移动文件
来源：http://hz.ydzc1.top/gtuqamkxqa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtbgqxtzuv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtodmlnwfo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtcnecqivs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtumitsflg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ywan-chungtsiang.top/gtsilaeppx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shangyingyoupin.top/gtofbxvbcj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtynquaxpd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sweek.top/gtwrtwievd.html

[F12] CSV 读写
来源：http://hz.yongpay.top/gtdzbtpzua.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtsjqrbtjw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydjk.org.cn/gtkmhitalb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinghuilouyu.cn/gtvrjmxoqr.html

TS:   // 同上
来源：http://hz.cashguo.top/gtdhphslax.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258888.top/gtagkjowew.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gthscarrlp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tian-w.cn/gtobzpsvir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.quarkkingdee.top/gtzymqgfha.html

================================================================================
来源：http://hz.yj20258.top/gtuscdmuwx.html

G. 面向对象
来源：http://hz.hysaishi.cn/gtncnxgifk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtytiqjefg.html

[G01] 定义类
来源：http://hz.bjfxy.top/gtcfyfrqii.html

Py:   class User: pass
来源：http://hz.gogol.net.cn/gtmawaynzq.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtwjaaljqw.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtgwdfzrlq.html

TS:   class User { name: string = ""; }
来源：http://hz.mhx1999.top/gthqxmzmaz.html

Java: class User {}
来源：http://hz.mhx1999.top/gtkdekcwos.html

Go:   type User struct { Name string }
来源：http://hz.xingfuxueyuan.xyz/gtspcwuizj.html

Ruby: class User; end
来源：http://hz.hnxiangtu.top/gtkrnqpqye.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtsoyiwion.html

[G02] 构造函数
来源：http://hz.xuanzx.com/gtdotrqyai.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtlxxsugag.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gteizvoxek.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.redwolf501.top/gtrepehzbk.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gtlcwkkxtc.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gtwqgpvysw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.0kj1m.cn/gtpcwdiogc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhengqikj.top/gtxitdvnho.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtjwtbymwy.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtkgqrnjfj.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gteacagvvi.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gtqkrumfjw.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtltjcnfrn.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtyyxaohqw.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtvkixmemo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtwbndaote.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gtcfkywand.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtadggrdxo.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtogzgfche.html

Py:   def greet(self): return self.name
来源：http://hz.ppjwa.cn/gtzbkirifz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtytzbwczq.html

JS:   greet() { return this.name; }
来源：http://hz.hfpthk.cn/gtmxjwksdm.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258888.top/gthodrdiia.html

Java: String greet() { return name; }
来源：http://hz.tianlin.xyz/gtgztqlghm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtkyfkhyro.html

Ruby: def greet; @name; end
来源：http://hz.vqdsnc.cn/gtadtiryqb.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtytqelfrj.html

[G05] 继承
来源：http://hz.ybcxt.top/gtlmpnthpm.html

Py:   class Admin(User): pass
来源：http://hz.52xcode.cn/gttjwciqzv.html

PHP:  class Admin extends User {}
来源：http://hz.cashguo.top/gtqpxhezcd.html

JS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gtewhejecq.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtgqqiuhib.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtdfoxnafl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgfzy.top/gtlcodrhfb.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtnmmmycfr.html

C#:   class Admin : User {}
来源：http://hz.tanke756.top/gtcuyyrqdg.html

[G06] 重写方法
来源：http://hz.ivvv.top/gtyphgqrli.html

Py:   def greet(self): return "admin"
来源：http://hz.yueranfly.top/gtkjcfoirw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtnnyheawt.html

JS:   greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtwnkymmdu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtrgbpzhps.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pycfn.com/gtlhfyqaex.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sysykeji.top/gttbtwwgaa.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gteaqsswxy.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtnxdgccqu.html

[G07] 调用父类方法
来源：http://hz.feifeiyinyue.top/gtkmgrpwzy.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtejrggkeg.html

PHP:  parent::greet();
来源：http://hz.xuetiantiany.cn/gtsfirdzei.html

JS:   super.greet();
来源：http://hz.chenlongwang.top/gtzgrtrinv.html

TS:   super.greet();
来源：http://hz.cashguo.top/gtemvgdisu.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtaigrywrg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yongpay.top/gtdgbldrpm.html

Ruby: super
来源：http://hz.yongpay.top/gtvpyosqbq.html

C#:   base.Greet();
来源：http://hz.aibaodan.cn/gtzgfjcwob.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gtrbbmbqni.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hongshengwenyu.top/gtdmlvoeat.html

PHP:  public static function f() {}
来源：http://hz.birdmap.top/gthsimiyxd.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gtqxsluccy.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtarliwznd.html

Java: static void f() {}
来源：http://hz.yueranfly.top/gtcqnsnufa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtwxpkfzsp.html

Ruby: def self.f; end
来源：http://hz.nwbrower.top/gtwnoiurpv.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtdgmrupet.html

[G09] 接口 / 抽象类
来源：http://hz.ydzc1.top/gtajhpbwmv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jyoumei.cn/gtuxmvvslg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj202588.top/gtwgpmdxtm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtbakshfww.html

TS:   interface Shape { area(): number; }
来源：http://hz.kuanghao11.cn/gtawipdyzi.html

Java: interface Shape { double area(); }
来源：http://hz.ywan-chungtsiang.top/gtgscdaijk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gtqbjgqxag.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtjghrkafr.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtauibfowr.html

[G10] 访问控制
来源：http://hz.hongshengwenyu.top/gtthwygczj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangshuangyany.cn/gtmmpwurag.html

PHP:  public / protected / private
来源：http://hz.jyoumei.cn/gtojqefjlb.html

JS:   #private 字段；其余公开
来源：http://hz.nanxinkj.top/gtwkfhzowb.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtkhqwvhot.html

Java: public / protected / private / 默认包级
来源：http://hz.xuetiantiany.cn/gtboubsksz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtqzvgcmuy.html

Ruby: public / protected / private
来源：http://hz.zhixingplan.top/gtrsfkejlv.html


<!-- 参考信息 -->