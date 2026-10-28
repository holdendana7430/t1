代发 wailian999

Ruby: s.reverse
来源：http://hz.xinyue.icu/gtfhbcoobn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtpuexvxgt.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtqpvdbnoo.html

Py:   s.count("a")
来源：http://hz.dashuyun.cn/gtyefmeyga.html

PHP:  substr_count($s, "a");
来源：http://hz.hnxiangtu.top/gtnkkxuxpc.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtqfhesjap.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtqttykwtm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.snrcjt.cn/gtaqoycqui.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gtgxvvgfuv.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtulniehnf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhijiandao.cn/gtnifdnanz.html

[E13] 逐字符遍历
来源：http://hz.sysykeji.top/gtiesuerwb.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtritrfwjj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.iojbl.cn/gtfkumkbpy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhiwuduotai.top/gtdevmsxoq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtznmzqjot.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.havefunace.top/gtufrlfjya.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jlsjyb.cn/gtylreszib.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nwbrower.top/gtwsyqcbpe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cdnleiting.top/gtwkaggkan.html

[E14] URL 编码与 Base64
来源：http://hz.pengpengdd.cyou/gtkuljoquz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hywenlv.cn/gtjcvtfyti.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gotoacloud.top/gtikqbwtkl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.birdmap.top/gtlefdhngx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtclhmbevx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnqzz.top/gtjwiwlcfk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhoulong.xyz/gtlfuzywwz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daria6918.cn/gtpjndvgez.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtlcwjejel.html

[E15] HTML 转义 / 反转义
来源：http://hz.quarkkingdee.top/gtcswfnrwb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gttfdkoedo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nwbrower.top/gtltcphkki.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtzioqdbdx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtvfcmwqec.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenlongwang.top/gtpvsvehrn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtmwsyjqos.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gtsqqobtpz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtmahdcuqh.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtnqogllla.html

Py:   f"{1234567:,}"
来源：http://hz.daria6918.cn/gtwouymryy.html

PHP:  number_format(1234567);
来源：http://hz.vqdsnc.cn/gtchfxuerd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtfqscigea.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtadxxbgce.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.birdmap.top/gtnrhvcxpp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgufenzy.top/gtmsmxkvzz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hfpthk.cn/gtmqzzheqa.html

C#:   1234567.ToString("N0")
来源：http://hz.chenlongwang.top/gtfyaniirk.html

[E17] 首字母大写
来源：http://hz.chenlongwang.top/gtsfaxnohm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtunhhyvuh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhixingplan.top/gthzabryiq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtsdlsofge.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gthymqhxkt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.andypj.xyz/gtorqsgcdz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dianchejie.cn/gtxycardwi.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtqmdyeqth.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhongyouzk.top/gtcynegmuu.html

[E18] 模板占位符替换
来源：http://hz.jlsjyb.cn/gtxadelrxc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.andypj.xyz/gtasnbnsin.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fzhhl.top/gtxhxiemxa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtjkswyhwz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtasvuduog.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtxigzzcvd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenjidiqi.icu/gtqtjsvxjx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shangyingyoupin.top/gtjdahheoh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xingfuxueyuan.xyz/gtcudafwcv.html

[E19] 多行文本按行拆分
来源：http://hz.cqqwz.cn/gtdxqoyynz.html

Py:   s.splitlines()
来源：http://hz.ivvv.top/gtywalgpcw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenjidiqi.icu/gtiawtsbyr.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtqpxzshlu.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtgdsuweov.html

Java: s.lines().toList()
来源：http://hz.chenzaomai.com/gtvuoqpaon.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj202588.top/gtfbhcmnjj.html

Ruby: s.lines
来源：http://hz.yj20258888.top/gtfuroujzp.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtxsaupstj.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gthuzuigmv.html

Py:   if not s:
来源：http://hz.yvedp.cn/gtpvjpxvvc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtdhzxswob.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guowangkeji.top/gtgvlrvkiw.html

TS:   if (s === "") {}
来源：http://hz.ydjk.org.cn/gtepaaratz.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtqxcjnzyi.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtavvplqir.html

Ruby: if s.empty?
来源：http://hz.hnxiangtu.top/gtllmbsdcp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gtfuexgsis.html

[E21] 超长截断加省略号
来源：http://hz.pengpengdd.cyou/gtkclgcgon.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtweqqmubk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gtvjtphkkm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtaqswaegp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtenllrhaq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtbovvzfkz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtbyxqymfi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cashguo.top/gtsocmmphz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guowangkeji.top/gtufnobwax.html

[E22] 字节长度与字符长度
来源：http://hz.cashguo.top/gtnomvqxmq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuanzhike.top/gtxomqnymy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtimfdyifa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtlbfqwhwx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtpavafvlp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtwapanxfu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhongyouzk.top/gtvtffkhya.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtydhlbpoa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtqajeetoz.html

================================================================================
来源：http://hz.havefunace.top/gthyuyuwby.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtecbbqrrh.html

================================================================================
来源：http://hz.zdqjudy.top/gtlglpsxej.html

[F01] 读取整个文件
来源：http://hz.fzhhl.top/gtrryyjhpk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.smart0.xyz/gtsgzcvlwj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtsslaytvv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtdeezsbtb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fzhhl.top/gtdtcjoawe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtcdwkghkn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinghuilouyu.cn/gthzyejspx.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtonmbgvgz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yongpay.top/gtuhjzculi.html

[F02] 逐行读取文件
来源：http://hz.zhengqikj.top/gtsxnizvoo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aibaodan.cn/gtrezueknb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shangyingyoupin.top/gtxvwviwco.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtztlwtbbu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtdnyqqavn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtwggtuhbh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtwvtxrcif.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtchfphfnt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.meibo888.top/gtxizppxjx.html

[F03] 写入文件（覆盖）
来源：http://hz.pengpengdd.cyou/gtjudniqkq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.52xcode.cn/gtziyagsmk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yonumen.top/gtgldcgbut.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtorjlanms.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtvnfojqbi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gtkfhijntr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtqfvhlter.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.bjfxy.top/gtjeivddqd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yonumen.top/gttvivnkfe.html

[F04] 追加写入文件
来源：http://hz.zhoulong.xyz/gtuuyvtyox.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtuukbunqh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.c1oappe.top/gtgiayfmag.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtwsuqswvx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtnhnhdcgh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuxming.cn/gtujtfcmed.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtajcoqsaj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hfpthk.cn/gtgufjnrhk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jyoumei.cn/gtqrypiduc.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gtnubytixl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuetiantiany.cn/gtascequqc.html

PHP:  file_exists("a.txt");
来源：http://hz.fengsongda.top/gteiyhcnsv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gttlollyuf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gttcncrhbs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtyuwadxhr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtvxsiqmin.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gteruytokx.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258888.top/gtgfomefos.html

[F06] 删除文件
来源：http://hz.sweek.top/gtskylvkuz.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtylpaghoe.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtkonwfofb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtcdigijfy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtzqougtyz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtmwthrita.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtvmrlsmwl.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gthxkcasyj.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtzggvomaw.html

[F07] 创建目录（含多级）
来源：http://hz.gotoacloud.top/gtqnpyquru.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aibaodan.cn/gtupwezvep.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dashuyun.cn/gtonffdnjc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtxxznzjoo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtezvpzglp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhongyouzk.top/gtkdygjvkr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.c1oappe.top/gtqyitmycr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jyoumei.cn/gtnwxeeypl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuxming.cn/gtyblefvwm.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtvqzbjumy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtxhqbygev.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtfaftvrii.html

JS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtlosjmfff.html

TS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtqvboglod.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtforzeogf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jlsjyb.cn/gttjjuiipj.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtvbxglcnu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hysaishi.cn/gtpbdkliqk.html

[F09] 获取文件大小
来源：http://hz.yongpay.top/gtiovdlxfv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gtxukvcvxj.html

PHP:  filesize("a.txt");
来源：http://hz.dashuyun.cn/gtsuuhmmcy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtmxevvmrc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtveuhabbm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtnbsgyjke.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.bjfxy.top/gtyycjigrd.html

Ruby: File.size("a.txt")
来源：http://hz.zhijiandao.cn/gtjfjcgtra.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtiyajxzab.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gttnprbbqf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gteqvjyovt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gtfyhjinki.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtxofedgvt.html

TS:   path.extname("a.txt")
来源：http://hz.ybcxt.top/gtripyvbks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenzaomai.com/gtqczgueme.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zdqjudy.top/gtjleochxf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtkoskprqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gtnpxwajgz.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtszncqgvi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtgfquacqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtqjuaflah.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gthxpctksh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtwevekrxn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhijiandao.cn/gtwjvzhzth.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtytdzyptm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtqylkapps.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtpgjvjiyt.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gtnqqvmkhh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gthmbfqdhj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtspqcscop.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangtech.top/gtcnsqmqvr.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtwgcwafff.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtesqzwdqx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hysaishi.cn/gtcnirgzaf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jianghu66.top/gtihxjjkkp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gthgjnktxk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttvqbwflv.html

G. 面向对象
来源：http://hz.yongpay.top/gtxaanfkke.html

================================================================================
来源：http://hz.chenzaomai.com/gtbetrzmjn.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtnkdbcbkj.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gtvrxhkzsj.html

PHP:  class User {}
来源：http://hz.hfpthk.cn/gtinelfgbx.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtgzpqqhap.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtmqexcpfl.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtebsubgau.html

Go:   type User struct { Name string }
来源：http://hz.jqgfzy.top/gtogfmfglc.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtjvmxvcut.html

C#:   class User {}
来源：http://hz.ppjwa.cn/gtyjqivizl.html

[G02] 构造函数
来源：http://hz.yj20258888.top/gtdtxpqios.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtebrbvwzz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtpinyuoia.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtuueecvsf.html

TS:   constructor(public name: string) {}
来源：http://hz.zhongyouzk.top/gtzxivxisy.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtgnhwlxti.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxinkj.top/gtqxcderzn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yueranfly.top/gtwmgxgzad.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fengsongda.top/gtepzzkqmx.html

[G03] 实例属性
来源：http://hz.jyoumei.cn/gtbognzdxy.html

Py:   self.name = "x"
来源：http://hz.jianghu66.top/gtfdmyrojf.html

PHP:  public string $name = "x";
来源：http://hz.hywenlv.cn/gtuxfdinel.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtvotoxjjm.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtdvmekltk.html

Java: private String name;
来源：http://hz.pengpengdd.cyou/gtyubsgvsh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtgvgwgmtc.html

Ruby: @name = "x"
来源：http://hz.havefunace.top/gtoynltpgq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangshuangyany.cn/gtxiqrphtm.html

[G04] 定义方法
来源：http://hz.shuidangran.top/gthloitonm.html

Py:   def greet(self): return self.name
来源：http://hz.quarkkingdee.top/gtazfdhwgn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtvbpbpjdh.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gtnprouplx.html

TS:   greet(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtsxtxvvxg.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtfyzndsgz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shzxlz.cn/gtlgbdbepy.html

Ruby: def greet; @name; end
来源：http://hz.haohaochexian.top/gtqcjipwsy.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigfzy.top/gtzfzwxzad.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtsasiqjqp.html

Py:   class Admin(User): pass
来源：http://hz.andypj.xyz/gtygjssutu.html

PHP:  class Admin extends User {}
来源：http://hz.svipenyu.cn/gtccyyuxyp.html

JS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtpcqqdgaf.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gttscwxqox.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtkqamdehg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xingfuxueyuan.xyz/gtmjkhmmmr.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtrqyxvtjt.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtddzcfmbw.html

[G06] 重写方法
来源：http://hz.gzhubu.top/gtlsphhbvp.html

Py:   def greet(self): return "admin"
来源：http://hz.gaohongyu789.top/gtahwmbsow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtgpxqgzbg.html

JS:   greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gttwtrijfg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtvdtywkzs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtntfywojv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtosowweht.html

Ruby: def greet; "admin"; end
来源：http://hz.gogol.net.cn/gtrtsvvpwt.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangtech.top/gtcwgynejy.html

[G07] 调用父类方法
来源：http://hz.jyoumei.cn/gtmgnxuvdz.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtxenebzif.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtqqxjwlsn.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtqudtrwgu.html

TS:   super.greet();
来源：http://hz.jiagoushi.top/gtnbafdhtc.html

Java: super.greet();
来源：http://hz.yj202588.top/gtanqsjwwu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cashguo.top/gtuhnldatd.html

Ruby: super
来源：http://hz.fengsongda.top/gtcckpozfs.html

C#:   base.Greet();
来源：http://hz.aibaodan.cn/gtsvdvxvpq.html

[G08] 静态方法与属性
来源：http://hz.bjfxy.top/gtdwifddjb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtlhpoqnjd.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtdeucukgy.html

JS:   static f() {}
来源：http://hz.wangshuangyany.cn/gtoeydjzoa.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtescotnol.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtgaiqckhg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dianchejie.cn/gtewlqpwht.html

Ruby: def self.f; end
来源：http://hz.shzxlz.cn/gtqkvudfbn.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtmveekjww.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtklqfspxz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnqzz.top/gtpbdrhchr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fengsongda.top/gtkbhgoqss.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtbtcmfabm.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gtosuvortp.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtrsrmmiin.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtlzobfhir.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ywan-chungtsiang.top/gtdnjesfxg.html

C#:   interface IShape { double Area(); }
来源：http://hz.ppjwa.cn/gtnjpesdow.html

[G10] 访问控制
来源：http://hz.jinqigfzy.top/gtkiuyqfom.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtexzyfzfy.html

PHP:  public / protected / private
来源：http://hz.zhengqikj.top/gtwgsvvlhr.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtxnemgpte.html


<!-- 参考信息 -->