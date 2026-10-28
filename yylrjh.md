代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.xylfe.cn/gtnmfoxwwo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydzc1.top/gtiwgddjaq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtsypmzwou.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gtyuoftfci.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tanke756.top/gtcclrsnra.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.andypj.xyz/gtjoshlggz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ehwqpu.com/gtfidgmabd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuanzhike.top/gtgzsxtrlj.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gtgpkxzgom.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtjrqbshet.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj20258888.top/gtskqgbyam.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hywenlv.cn/gtjpccsncj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ywan-chungtsiang.top/gtpfubfgru.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtogqzbuyy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yonumen.top/gtbjbmcwau.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.vqdsnc.cn/gtjpivivxg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtutwdgizw.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtmvvylnhf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhoulong.xyz/gtuvgtsfcj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenjidiqi.icu/gtnlmoogtl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gtlzdcvaak.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgfzy.top/gtfplyxukq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aizwys.cn/gtejbblaxw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gtybpstteo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhoulong.xyz/gtucodrafx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.iojbl.cn/gtkdumnoga.html

[E16] 数字千分位
来源：http://hz.wangshuangyany.cn/gtomsdcepf.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangtech.top/gtjhfzonwj.html

PHP:  number_format(1234567);
来源：http://hz.c1oappe.top/gtaaarwkfq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtslkqjhks.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtlejxdvqy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtppcfexyl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hywenlv.cn/gtdzynqaex.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhixingplan.top/gtfwpqypje.html

C#:   1234567.ToString("N0")
来源：http://hz.mhx1999.top/gtahcwfgxi.html

[E17] 首字母大写
来源：http://hz.wangshuangyany.cn/gtrrbqyfor.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtfnoawwls.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jyoumei.cn/gtyyhuypvh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtvnithpha.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtpfzoocrg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yonumen.top/gtxhlhhkwh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ivvv.top/gtxzumdbxr.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gtcjikuumu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigfzy.top/gtqsgcgxck.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtgviffrds.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yongpay.top/gtvlpvnpbw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigfzy.top/gtlllnboid.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtuquecqyh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtzzpsogow.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtpvyeauxh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sxryk.cn/gtyhmwbpyv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhongyouzk.top/gtffqvhyio.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtslparpmy.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258888.top/gtblhxcxnf.html

Py:   s.splitlines()
来源：http://hz.vqdsnc.cn/gtsglritfa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.svipenyu.cn/gtqkbogtnb.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtypmndikv.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtdhgjesmy.html

Java: s.lines().toList()
来源：http://hz.52xcode.cn/gtxhjfbrsr.html

Go:   strings.Split(s, "\n")
来源：http://hz.gaohongyu789.top/gtgwtfpnkq.html

Ruby: s.lines
来源：http://hz.xuanzx.com/gtouilhstz.html

C#:   s.Split('\n')
来源：http://hz.jinqigfzy.top/gttboaqxcy.html

[E20] 判断字符串是否为空
来源：http://hz.yonumen.top/gtwcceqono.html

Py:   if not s:
来源：http://hz.nwbrower.top/gtpmlzigda.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.9152youxi.cn/gtbjzdyzjg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhijiandao.cn/gtvxzyexej.html

TS:   if (s === "") {}
来源：http://hz.yongpay.top/gtqraozrkl.html

Java: if (s.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtqrvcsikh.html

Go:   if s == "" {}
来源：http://hz.feifeiyinyue.top/gtnixzjjwf.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gtwheyodbf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigfzy.top/gtmmepcsxp.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtzgizgeyf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtrudvbhxn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtlsotvpyf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtfueiitto.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtpfmvznya.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtxgrkatjg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tian-w.cn/gtpclizdai.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtwwoohneg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtuqvmozke.html

[E22] 字节长度与字符长度
来源：http://hz.chenzaomai.com/gtqjpjstia.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hysaishi.cn/gthzsykmre.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtdkgkqufk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtractjymn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtrnpdrsax.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shanyushiyangkeji.top/gtjllldvkd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gtvezgzwey.html

Ruby: s.bytesize;  s.length
来源：http://hz.zdqjudy.top/gtvyebwxrm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtdkkxqjub.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpirsycyp.html

F. 文件与目录
来源：http://hz.0kj1m.cn/gtuhtzuykc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtoxrnevoc.html

[F01] 读取整个文件
来源：http://hz.gaohongyu789.top/gtgkuncslt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.0kj1m.cn/gtxkrurwcx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtyohabgjj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tanke756.top/gtwsmlvgjg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gttbympcjp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtjqphiudr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gthntpxwoq.html

Ruby: File.read("a.txt")
来源：http://hz.jyoumei.cn/gterlkpmmj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtgizoqrsk.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gtjeybtyvj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtuvlfpwqa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinghuilouyu.cn/gtwfjdxlhc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtqvhoxnzg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gteihavooh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtnbxfrnqj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtbcsmpvjh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtiwpgkxqv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tanke756.top/gtevefqqtb.html

[F03] 写入文件（覆盖）
来源：http://hz.chenlongwang.top/gtzwpvxfwj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zycfv.cn/gthpoyxevk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj202588.top/gttfgqhdcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtzyobbvvr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtcjkoxxyd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fzhhl.top/gtrxruduek.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fzhhl.top/gtokaxqmnl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gtozvjtbml.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtkowtziti.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtlloufczw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtdcfadrhn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhaomingkeji.xyz/gtsfeeplxn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtqfrnauno.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtikcmnshy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtposrifbi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.quarkkingdee.top/gttckrgyjf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtncrbqzxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gtlevuolps.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtqjvapzik.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtoyrrgpzd.html

PHP:  file_exists("a.txt");
来源：http://hz.feifeiyinyue.top/gtpzohpxxw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtkvmncxce.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtpanadwpi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtywfaqayy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtqlslfvgz.html

Ruby: File.exist?("a.txt")
来源：http://hz.sweek.top/gtpwohzbnv.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtdtbjiivd.html

[F06] 删除文件
来源：http://hz.shzxlz.cn/gtutwecdyq.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtpykujqsf.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gtuevjygmz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtivddegti.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtajhuxjzb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gthibcwxdv.html

Go:   os.Remove("a.txt")
来源：http://hz.sufxvd.cn/gtxnxavehm.html

Ruby: File.delete("a.txt")
来源：http://hz.jqgufenzy.top/gtvicetqjf.html

C#:   File.Delete("a.txt");
来源：http://hz.feifeiyinyue.top/gtakvyknaj.html

[F07] 创建目录（含多级）
来源：http://hz.zhijiandao.cn/gthfcarwzf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.c1oappe.top/gturioizga.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtdghutlmx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gthcrghouc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtnrinqflg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258.top/gtxijlbjkj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtfahwcfpn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhiwuduotai.top/gthckgkqlo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gtrletjvvx.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtvjclmign.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtsnbpjvoa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pycfn.com/gtfqnxkgsv.html

JS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtbcuzcatl.html

TS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtjyorddfv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtpwdskcvm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtozugeaky.html

Ruby: Dir.children("dir")
来源：http://hz.xziqi.cn/gtuzneugkl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gteiiaguug.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtlcdyrsrv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenjidiqi.icu/gtplvpnklp.html

PHP:  filesize("a.txt");
来源：http://hz.dianchejie.cn/gtefwmorer.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtyitulaea.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yonumen.top/gttzjdplfa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtwvwcnhbg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shzxlz.cn/gtyewnimbe.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtggemxuqf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nwbrower.top/gtzjkbudby.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dianchejie.cn/gtpalwxlam.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtftsuktve.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtcchjqcrs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtyunnlscp.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtaeqyzxdk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sweek.top/gtvhrdpbbu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtjahvdskd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtoufmetrk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtohtlxwsb.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtuhwvgzeh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtbfidaykh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtyyddevkw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtsrfwktqs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtwifbkxmp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yanxiufei.cn/gtjsfmuwrc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yongpay.top/gtntpomifd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtsqnohuvi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sweek.top/gtonoqgmyc.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtjbwtvssh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtuvrygimo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtegcelscf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtfnixxqcv.html

TS:   // 同上
来源：http://hz.yuxming.cn/gtuajhecjb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtxsofcyot.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtqjelyiyf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yongpay.top/gtuofqqzht.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtmebitwhr.html

================================================================================
来源：http://hz.ybcxt.top/gtixxombpz.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtzqbttcrw.html

================================================================================
来源：http://hz.0kj1m.cn/gtwbbudhpb.html

[G01] 定义类
来源：http://hz.yuxming.cn/gtfokyzixi.html

Py:   class User: pass
来源：http://hz.dianchejie.cn/gtcybtfvqr.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtrotnokxg.html

JS:   class User {}
来源：http://hz.guowangkeji.top/gtlovsnuhl.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtwciunytg.html

Java: class User {}
来源：http://hz.redwolf501.top/gtuimbbmor.html

Go:   type User struct { Name string }
来源：http://hz.52xcode.cn/gtgurmqbnq.html

Ruby: class User; end
来源：http://hz.xuetiantiany.cn/gtoxusiate.html

C#:   class User {}
来源：http://hz.yongpay.top/gtaumwlqdd.html

[G02] 构造函数
来源：http://hz.yueranfly.top/gtzunhwmqx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gtgxcngkpx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.meibo888.top/gtcovcpmca.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtmetwhajc.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gtgqpvlgfu.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuxming.cn/gtmdllutqr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtskjfknsb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gttjbovzqp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtqvodnyib.html

[G03] 实例属性
来源：http://hz.jinqigufen.top/gtxbpfvnri.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtclktgvwl.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtwdfeftes.html

JS:   this.name = "x";
来源：http://hz.gotoacloud.top/gtbitmuegc.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtgskrgixq.html

Java: private String name;
来源：http://hz.jinyuanbaomall.cn/gtwessmjoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnxiangtu.top/gtgnnyxkbs.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gtnhqjwefs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yongpay.top/gtlpooinwz.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtplwyyuis.html

Py:   def greet(self): return self.name
来源：http://hz.hysaishi.cn/gtxydyperw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtayziunac.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gtyurxjxkn.html

TS:   greet(): string { return this.name; }
来源：http://hz.yvedp.cn/gtfucxihbu.html

Java: String greet() { return name; }
来源：http://hz.xylfe.cn/gtsosjrecv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtibtpjlth.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangtech.top/gtylnlbpzp.html

C#:   public string Greet() => Name;
来源：http://hz.zycfv.cn/gtcavrcllm.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtcxlfbcer.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtsjqfalaa.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtvyiihiay.html

JS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtwypqmgzw.html

TS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtymmlxsfp.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtsfjrqctj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtvoxmwjof.html

Ruby: class Admin < User; end
来源：http://hz.zhiwuduotai.top/gtdiupqzzb.html

C#:   class Admin : User {}
来源：http://hz.havefunace.top/gttwuginnk.html

[G06] 重写方法
来源：http://hz.gotoacloud.top/gthfapsnma.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtrlncisan.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtrkhsyrii.html

JS:   greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtmofisuul.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtgqzrgeso.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yonumen.top/gtsickhqqz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtttwrfzjo.html

Ruby: def greet; "admin"; end
来源：http://hz.gaohongyu789.top/gtfducnmkc.html

C#:   public override string Greet() => "admin";
来源：http://hz.jyoumei.cn/gttcibxrwy.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtnyqitkoc.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gtzkxyjnit.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtiutmdtpq.html

JS:   super.greet();
来源：http://hz.cheryme.top/gtazyczowj.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtfxhkaooq.html

Java: super.greet();
来源：http://hz.sweek.top/gtsroqdjdd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtuundlbxt.html

Ruby: super
来源：http://hz.andypj.xyz/gtjergkphj.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtduequyph.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtnlstdfjn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.bjfxy.top/gtlqsrjkpa.html

PHP:  public static function f() {}
来源：http://hz.nanxinkj.top/gteukezgue.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtfibvrsaj.html

TS:   static f(): void {}
来源：http://hz.xylfe.cn/gtjtfdtbxw.html

Java: static void f() {}
来源：http://hz.nanxinkj.top/gtthhqufsd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtofvavdeb.html

Ruby: def self.f; end
来源：http://hz.yj20258888.top/gtlbwpgaou.html

C#:   public static void F() {}
来源：http://hz.chenzaomai.com/gtdbffxktm.html

[G09] 接口 / 抽象类
来源：http://hz.jlsjyb.cn/gtuldfhxgi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.0kj1m.cn/gtndbhzjuo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.vqdsnc.cn/gtnvkabwiz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gttexceyiy.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtfpyyaada.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtycvnjitn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenjidiqi.icu/gtteofguaw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtsxtxxcqg.html

C#:   interface IShape { double Area(); }
来源：http://hz.andypj.xyz/gtntyvsuub.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtylsvdsli.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cucudq.cn/gthoyysrqr.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtdwjmmoxs.html

JS:   #private 字段；其余公开
来源：http://hz.jlsjyb.cn/gtmohpzorv.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gtmagvemnf.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtesbqtebg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtjwqaspkg.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtaplpncik.html

C#:   public / protected / private / internal
来源：http://hz.pycfn.com/gtzeqsyzhd.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtwyzzcqvh.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtfgjqtpug.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtzslsvjxo.html

JS:   get name() { return this._name; }
来源：http://hz.cashguo.top/gtihyvzzfm.html

TS:   get name(): string { return this._name; }
来源：http://hz.bjfxy.top/gtlpktyltm.html

Java: public String getName() { return name; }
来源：http://hz.xuetiantiany.cn/gtadblfpgd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtxlbzfnbk.html


<!-- 参考信息 -->