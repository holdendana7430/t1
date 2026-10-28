代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtakchycpp.html

TS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtqzvlkqum.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ybcxt.top/gtyffiafox.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sufxvd.cn/gttyucessb.html

Ruby: s.reverse
来源：http://hz.ybcxt.top/gtiyddxplh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtuhhuumfx.html

[E12] 统计某字符出现次数
来源：http://hz.hysaishi.cn/gtepetjtvs.html

Py:   s.count("a")
来源：http://hz.shanyushiyangtech.top/gtmpxvznjp.html

PHP:  substr_count($s, "a");
来源：http://hz.jyoumei.cn/gtnxhfvljn.html

JS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtgmsbahhp.html

TS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtojakgdpg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xziqi.cn/gtpgzxvtsm.html

Go:   strings.Count(s, "a")
来源：http://hz.wangdashe.top/gtzcjcxvae.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtdjrjutrm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtcskgtofa.html

[E13] 逐字符遍历
来源：http://hz.dianchejie.cn/gtfjujkyca.html

Py:   for ch in s: print(ch)
来源：http://hz.0kj1m.cn/gtfwtahnwm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtrxtsnblv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtwykhhrjn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtsstgzaxp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hfpthk.cn/gtdyhlbqtx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.0kj1m.cn/gtioraycrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yanxiufei.cn/gtjiocnooo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.mhx1999.top/gtqhhwagdt.html

[E14] URL 编码与 Base64
来源：http://hz.xuetiantiany.cn/gtfioqqffr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gtsrwchuef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuxming.cn/gtdnozckwj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gtgohdzasb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtqauuxzjq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yueranfly.top/gtvonogrml.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gtwzgatypl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hammf.cn/gtlsqrfgeo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtqngwushv.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gttdiqjxdq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.svipenyu.cn/gtxvqccqgt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zycfv.cn/gtnuzeltvh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gtptsasudp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuanzx.com/gtayjzdond.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxuanxn.top/gtdafrkfxs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenjidiqi.icu/gtmkmiirsk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtosfgxams.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.redwolf501.top/gtswojwcby.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtmuxbaapq.html

Py:   f"{1234567:,}"
来源：http://hz.gotoacloud.top/gtcgkzbtfe.html

PHP:  number_format(1234567);
来源：http://hz.52xcode.cn/gtdwaqbqxf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gttfmnslmc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtobkcgsjl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuanzx.com/gtovaovsqe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgfzy.top/gtswymsgjg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gtdylayhyb.html

C#:   1234567.ToString("N0")
来源：http://hz.birdmap.top/gtimewlfbt.html

[E17] 首字母大写
来源：http://hz.jinghuilouyu.cn/gtivkryslj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.quarkkingdee.top/gthmnjywos.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.c1oappe.top/gtlushaign.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtdmuzvsme.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtkdzupohs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtskvoptes.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.bjfxy.top/gtbxvrsvtf.html

Ruby: s.capitalize
来源：http://hz.sxryk.cn/gtncjpfjjo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuxming.cn/gtzjtsyuni.html

[E18] 模板占位符替换
来源：http://hz.sweek.top/gtmtmbgevo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jyoumei.cn/gtccncdcxy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtygrdujzy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtosadtdxr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtqdnsgtoi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtdafuarxv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gtgccaasnw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jianghu66.top/gtusehcmlk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuetiantiany.cn/gtpcqyjsji.html

[E19] 多行文本按行拆分
来源：http://hz.yonumen.top/gtabwmbkkl.html

Py:   s.splitlines()
来源：http://hz.yj20258.top/gtbxdevpqv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258888.top/gtqkrlmmom.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtfrnlvodp.html

TS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtzbjaghkr.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtlkjmdewc.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gtbiolcobv.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtffowmuca.html

C#:   s.Split('\n')
来源：http://hz.yongpay.top/gtofvmebks.html

[E20] 判断字符串是否为空
来源：http://hz.smart0.xyz/gttobcypzs.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtwiqgyqyc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenzaomai.com/gtepqzdhxy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinghuilouyu.cn/gtvcfsjyje.html

TS:   if (s === "") {}
来源：http://hz.jqgfzy.top/gtxwzssyuk.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtdftqjgiw.html

Go:   if s == "" {}
来源：http://hz.zhoulong.xyz/gtvcnloqgz.html

Ruby: if s.empty?
来源：http://hz.zhaomingkeji.xyz/gtkhoezjei.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jianghu66.top/gthbypagox.html

[E21] 超长截断加省略号
来源：http://hz.xuanzx.com/gtweuvfina.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtpldtnytk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gtmrmyrolx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtlqeuazps.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtfchihedv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtcgwcutep.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gterklznrm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gttaptmliu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cdnleiting.top/gtswshlcoi.html

[E22] 字节长度与字符长度
来源：http://hz.feifeiyinyue.top/gtzpadnxbd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jianghu66.top/gtzmxpoblr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtewqqlzbt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xinyue.icu/gtkguihooz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gttpkkmcze.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtmnhpyglw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtdxaiklmo.html

Ruby: s.bytesize;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtswcbujiv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtwtdbgllj.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdqgacoep.html

F. 文件与目录
来源：http://hz.zhiwuduotai.top/gtbvguhyiu.html

================================================================================
来源：http://hz.0kj1m.cn/gtpvmotqoo.html

[F01] 读取整个文件
来源：http://hz.aizwys.cn/gtzyxhpvsg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xziqi.cn/gtdojriqph.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guannengcc.top/gtxvvpvloz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hfpthk.cn/gtdafrvfwl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtfewivgkc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtgirxonqt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hywenlv.cn/gtxhcsukjo.html

Ruby: File.read("a.txt")
来源：http://hz.ehwqpu.com/gtejuyzhqa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gtuapcnfue.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtucgkqfqn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.snrcjt.cn/gtgotepajp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnqzz.top/gtqfnptnsf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtuzkpwnst.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtlzldcuxo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtawbnryqp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fengsongda.top/gtlgawmjpy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.mhx1999.top/gtaerzxunh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuetiantiany.cn/gtrzhkpwuc.html

[F03] 写入文件（覆盖）
来源：http://hz.pengpengdd.cyou/gtdrhdzrqv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtzufhscir.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hammf.cn/gthauzwjkq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtvpiqgwwf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtjynrsewo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fengsongda.top/gtduejsutg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.guannengcc.top/gtyuovlruz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gticsxejdp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sxryk.cn/gtmexvgrfk.html

[F04] 追加写入文件
来源：http://hz.guowangkeji.top/gtkjkxtbza.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yanxiufei.cn/gtzvwerurf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangtech.top/gteodradmh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtangjjjsz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuxming.cn/gtrzqicaxd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xinyue.icu/gtdklqbvib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pycfn.com/gtsczdwoxb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtifgojtgz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gzhubu.top/gtshygajhw.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigufen.top/gtuuojgcia.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnqzz.top/gtvaajvnaq.html

PHP:  file_exists("a.txt");
来源：http://hz.ybcxt.top/gtuqokctuk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gttpcoihhr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtogiupskh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gttbxtrjek.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtfwicjmiu.html

Ruby: File.exist?("a.txt")
来源：http://hz.pycfn.com/gtrsyfaipg.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gthvqvopfx.html

[F06] 删除文件
来源：http://hz.zhoulong.xyz/gtlsuhatgf.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gtenduknre.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtzwccnget.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtxryedets.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtnzsiowoi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtvbznxbjw.html

Go:   os.Remove("a.txt")
来源：http://hz.ivvv.top/gtbtxtihej.html

Ruby: File.delete("a.txt")
来源：http://hz.mhx1999.top/gtumqxxqwl.html

C#:   File.Delete("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtyvxjxoht.html

[F07] 创建目录（含多级）
来源：http://hz.birdmap.top/gtddtvmfqz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jyoumei.cn/gtigdvqtdg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cashguo.top/gthzmacthw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtjsuebmyh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtqubnumhf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.snrcjt.cn/gtwrsanrhq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gtcdrunhcr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtjeilicde.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.havefunace.top/gtbxkjivlk.html

[F08] 遍历目录
来源：http://hz.zhoulong.xyz/gtwqgkyhkc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gtfwvjmzrn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydzc1.top/gtgnvbsvrk.html

JS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtcvkddljg.html

TS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtrslstomq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtjctmuqvq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.vqdsnc.cn/gtgdpjegbi.html

Ruby: Dir.children("dir")
来源：http://hz.fzhhl.top/gtrxzwaenl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.316326.xyz/gtmjgyefmb.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtlsxqaayd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gtonqynncj.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtwuknazuq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gtvaskssun.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtnihpaqkq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtuchceggy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtxklcbyrn.html

Ruby: File.size("a.txt")
来源：http://hz.feifeiyinyue.top/gtiumeqksn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gthktverpf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtwgflzkcv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtueywuzio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ivvv.top/gtuykwtfpa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtoxfwbjjc.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtfuwbsitm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.316326.xyz/gtgodwjmpo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtsrwafjvy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtmlzkgvzp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sxryk.cn/gtbggnbhdc.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtunzanfan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtxnuuabwc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258888.top/gtrxlcikap.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtmnfmznwv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtakndmzae.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtrtklxdmm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gtlsljoehe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtncghsxax.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtnnirgoks.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtfeyufpcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangdashe.top/gtbwntjdjs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xinyue.icu/gtshlepbhd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.quarkkingdee.top/gtmcbusnjc.html

TS:   // 同上
来源：http://hz.ppjwa.cn/gtxetlnxlm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fengsongda.top/gtaoxalrfl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yongpay.top/gtfoeudhnr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtleiywyzm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ybcxt.top/gtashbynxt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvlsxvhbu.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtrtetkzyn.html

================================================================================
来源：http://hz.ehwqpu.com/gtghqnkhdn.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtjgihakbw.html

Py:   class User: pass
来源：http://hz.havefunace.top/gtnwkhjxcs.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtzsmnmwgy.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtoyzxtvlv.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtgqroxupn.html

Java: class User {}
来源：http://hz.yuanzhike.top/gtbknhddhh.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtypdpdaoq.html

Ruby: class User; end
来源：http://hz.jinyuanbaomall.cn/gtdicwjdrg.html

C#:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtobvxkohl.html

[G02] 构造函数
来源：http://hz.jinyuanbaomall.cn/gtjbhtcrwj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gthusovced.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtsesksbdq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daria6918.cn/gtdnososzt.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtvbtwrkfk.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtvndjzeoe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtcucfkcmh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ivvv.top/gthamqhgoj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtheaktyqv.html

[G03] 实例属性
来源：http://hz.zdqjudy.top/gtctmxyovr.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gtjlplbcbd.html

PHP:  public string $name = "x";
来源：http://hz.quarkkingdee.top/gtjyumqvva.html

JS:   this.name = "x";
来源：http://hz.tian-w.cn/gtkkvzijtr.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtaftloqfj.html

Java: private String name;
来源：http://hz.shuidangran.top/gtnftlamdv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cqqwz.cn/gtmhoqwlgx.html

Ruby: @name = "x"
来源：http://hz.hysaishi.cn/gttcrhqcxx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fengsongda.top/gtabriijww.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtngmdhwwp.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtramljyar.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtwdhhldgr.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gthpeyjebc.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gtqpmcnkev.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtjvkqzqqo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gtayrxsynh.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtenfzxowl.html

C#:   public string Greet() => Name;
来源：http://hz.52xcode.cn/gtuagfmcwd.html

[G05] 继承
来源：http://hz.hnxiangtu.top/gtoeahnoij.html

Py:   class Admin(User): pass
来源：http://hz.zhaomingkeji.xyz/gtnailnjun.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtxyukmjtg.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtspfxoajj.html

TS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtgoygeksk.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtkidnexxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhoulong.xyz/gtikqplhlb.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtzpgyfaqf.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtamemnicp.html

[G06] 重写方法
来源：http://hz.xingfuxueyuan.xyz/gtnlgvpequ.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtciahdaho.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtigygvkqk.html

JS:   greet() { return "admin"; }
来源：http://hz.cheryme.top/gtvvmwnfuc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtdhkbkpdi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtiwhtrwzl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtcyyejjti.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtzxuyjujz.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gtetkarlct.html

[G07] 调用父类方法
来源：http://hz.hfpthk.cn/gtylhcbskj.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtcsgcntez.html

PHP:  parent::greet();
来源：http://hz.yuanzhike.top/gtssrjgfji.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtewtwvrkr.html

TS:   super.greet();
来源：http://hz.tian-w.cn/gtqklhiqfs.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtpaxupdlx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.0kj1m.cn/gtvushijsc.html

Ruby: super
来源：http://hz.ppjwa.cn/gtdoidnzsa.html

C#:   base.Greet();
来源：http://hz.feifeiyinyue.top/gtllrdzeqh.html

[G08] 静态方法与属性
来源：http://hz.jlsjyb.cn/gtmllrpeqp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtvgllhnmf.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtetagscrh.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtvpwruwkp.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangkeji.top/gtzbgntnfg.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtrkiozxbs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtmdfpsbyo.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtacgmoelz.html

C#:   public static void F() {}
来源：http://hz.hnxiangtu.top/gthneabace.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258.top/gtfgvpgkup.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtlxfsyvdy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ybcxt.top/gteomeddwt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtmaaaenet.html

TS:   interface Shape { area(): number; }
来源：http://hz.pycfn.com/gtsbfojstt.html

Java: interface Shape { double area(); }
来源：http://hz.316326.xyz/gteoldxmil.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gtbkuudesi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.snrcjt.cn/gtehomnmhr.html

C#:   interface IShape { double Area(); }
来源：http://hz.ivvv.top/gtocgysjjh.html


<!-- 参考信息 -->