代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gthvkozvps.html

[E11] 反转字符串
来源：http://hz.nwbrower.top/gtahspyclh.html

Py:   s[::-1]
来源：http://hz.andypj.xyz/gtdkxrbagc.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtsyrnjbrm.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtjujgbrkf.html

TS:   [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtzpsfrjze.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daxiang520.top/gtenwdjubc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gttwftuqwg.html

Ruby: s.reverse
来源：http://hz.shanyushiyangkeji.top/gtbghtuivt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtyraerwcn.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gtlwhtqzdb.html

Py:   s.count("a")
来源：http://hz.tanke756.top/gtkzplcnfp.html

PHP:  substr_count($s, "a");
来源：http://hz.shuidangran.top/gtpvfxofix.html

JS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtpecomplx.html

TS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtykhztnuf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.smart0.xyz/gtdwudcvkp.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtncqkzolj.html

Ruby: s.count("a")
来源：http://hz.redwolf501.top/gtggdizlbc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xingfuxueyuan.xyz/gtgtwzeltg.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gtkdtrwawb.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gtatpfzcao.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gtodnpgkii.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtsyqzrahc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtbblsukfh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cqqwz.cn/gtlhphezix.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tanke756.top/gtsfrkbecg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gtrjylxmge.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yueranfly.top/gttgjofwai.html

[E14] URL 编码与 Base64
来源：http://hz.tianlin.xyz/gtitlrawcs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hongshengwenyu.top/gthnspzcub.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shangyingyoupin.top/gtobzpovsf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.kuanghao11.cn/gtclfwscpx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtoulbvmjo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gttshtwcib.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.iojbl.cn/gtseruowvy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtkdrnplxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydzc1.top/gtynkdldub.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtrxqzturz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhijiandao.cn/gtagrozdfg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258888.top/gtsrwxgpkk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gtuowehgfi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hysaishi.cn/gtugfnhttz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dashuyun.cn/gtftbncmwa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtjdlhncsx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gthdfnyihj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtebfbfbnp.html

[E16] 数字千分位
来源：http://hz.52xcode.cn/gtgigonsnn.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtmnaiidqj.html

PHP:  number_format(1234567);
来源：http://hz.chenjidiqi.icu/gttnpqatgb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtwgffadfn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtynpniyhb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj202588.top/gtomqfrofn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xinyue.icu/gtvveahpbu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guowangkeji.top/gtqrokqmlg.html

C#:   1234567.ToString("N0")
来源：http://hz.hfpthk.cn/gtsfycvwsm.html

[E17] 首字母大写
来源：http://hz.jinyuanbaomall.cn/gtfzovpnwp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ywan-chungtsiang.top/gthylvxncr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtyisdtvdz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gthyvsjmqp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtjgytvbpu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gtogxtoist.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigufen.top/gtcswlqqmw.html

Ruby: s.capitalize
来源：http://hz.hnxiangtu.top/gttappfebv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cheryme.top/gtrdymognt.html

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gtnrvdzsjx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gtrquejilv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gtyakzabia.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtftkgucfr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gttwzndggv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtiijqchyx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fengsongda.top/gtuzbpmuba.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zdqjudy.top/gtisxuqulr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj202588.top/gtueodjczc.html

[E19] 多行文本按行拆分
来源：http://hz.hfpthk.cn/gtbweutuaz.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtitwdeimt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sysykeji.top/gtxbebqrdg.html

JS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gtqqzveydx.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtjkxlwane.html

Java: s.lines().toList()
来源：http://hz.gogol.net.cn/gttkyhxqgc.html

Go:   strings.Split(s, "\n")
来源：http://hz.gogol.net.cn/gtgfqodonb.html

Ruby: s.lines
来源：http://hz.shzxlz.cn/gtkvwpgvjr.html

C#:   s.Split('\n')
来源：http://hz.fengsongda.top/gtkiqwhilc.html

[E20] 判断字符串是否为空
来源：http://hz.smart0.xyz/gtsippfkqs.html

Py:   if not s:
来源：http://hz.daria6918.cn/gtpsfbsjde.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gotoacloud.top/gtdqfzmikq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.0kj1m.cn/gtyqpgoloh.html

TS:   if (s === "") {}
来源：http://hz.jqgfzy.top/gtbbfjbifh.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtqxtqgaya.html

Go:   if s == "" {}
来源：http://hz.316326.xyz/gtzjqdzlvs.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gtxnoayjbi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258.top/gtyrymchod.html

[E21] 超长截断加省略号
来源：http://hz.redwolf501.top/gtxlxmrsbe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtqmwzblmd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtichsukes.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtwqddgqyg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtirzxsnsx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtynqbtjgb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtezmfmygs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuanzhike.top/gtojtxfard.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.bjfxy.top/gtagwuhumu.html

[E22] 字节长度与字符长度
来源：http://hz.iojbl.cn/gtpezwkomi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ppjwa.cn/gtkkpfiomj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtuxeathts.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gttdrqhqiq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtkllxrnsd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtfadkddbr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtawqttezz.html

Ruby: s.bytesize;  s.length
来源：http://hz.jianghu66.top/gtatcnmzoa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yonumen.top/gtwpiwzgli.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgsteoaqf.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtholpjwbb.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwrlumrua.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtxbjpjtpb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtzaokrkro.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jyoumei.cn/gtxqpasumy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtkavfguva.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenlongwang.top/gtuiauwfbn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtlsdtrhwh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtltuqqweu.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtldqxceik.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.svipenyu.cn/gtnbqxdrso.html

[F02] 逐行读取文件
来源：http://hz.yj20258888.top/gttxqmzkjo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pengpengdd.cyou/gtdticfkpg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj202588.top/gtmleuzynb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtilhlsaeh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtujmyizej.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gthtjgeiyd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtyyogowqp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sufxvd.cn/gtcnprfpcb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnxiangtu.top/gtkxxguqvc.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgufenzy.top/gtomeddhxd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinyuanbaomall.cn/gttvpbhxoh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtkugosnki.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtewaymumx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtxfdazjzz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sysykeji.top/gtpryczvpw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenjidiqi.icu/gtxiqkxovd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cdnleiting.top/gtzylpoiup.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtaqezuoij.html

[F04] 追加写入文件
来源：http://hz.jqgufenzy.top/gtjbuejwmq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gthaalhetj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fengsongda.top/gtdpxloywn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtombggpoj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtpdfjqpsz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guannengcc.top/gtslhhaobp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ivvv.top/gtffjnqxfl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jlsjyb.cn/gtytnbksdv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shuidangran.top/gtadypvkga.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtijzribwy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtxuyqttte.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtjkpwswnk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtybhjlref.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtiiyruhmz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtjlmfkijm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuanzx.com/gtaoerchoe.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gttwuolbwo.html

C#:   File.Exists("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpnqiumic.html

[F06] 删除文件
来源：http://hz.andypj.xyz/gtokskperj.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtpqnxxjnd.html

PHP:  unlink("a.txt");
来源：http://hz.c1oappe.top/gtgggnxkbr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtnikxysse.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtayawbjpa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gthxbmsfjy.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtemirevfk.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtyxshqtnz.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gttmosdwox.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtkavmafno.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gtimtzgpoq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.aibaodan.cn/gtndkoznni.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gtdsqloibg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtavsbbtec.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhongyouzk.top/gtszbeadsq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.vqdsnc.cn/gtplpqjske.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangtech.top/gttnyoravx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtxzxdettc.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gthwdhqbbj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cdnleiting.top/gtgrnordpw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gthrgqsfec.html

JS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtgcmznkob.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtrbrccnzz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtwkisqtbm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yanxiufei.cn/gtqhokwubk.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtmxfnenpa.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtxumaecwd.html

[F09] 获取文件大小
来源：http://hz.tanke756.top/gtxugtmvzd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtplrddtym.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtueldmhcw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtwgerbsfq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtwpcwldrx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtlbuvcaby.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangdashe.top/gtmrilhdzb.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtjbsofezy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ivvv.top/gtmzdmwryr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jlsjyb.cn/gttrofcjbw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtdbldvbgb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtifdmjvhg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtgafmxoms.html

TS:   path.extname("a.txt")
来源：http://hz.hnqzz.top/gtgxwazbnr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtvzsklkrl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtxywgfvus.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtmryskqix.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydzc1.top/gtrfiqkibo.html

[F11] 复制与移动文件
来源：http://hz.gotoacloud.top/gtxqkvgkib.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtooijelkc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cheryme.top/gtvppcjtry.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtlhlolpkt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtovqbtwgz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxinkj.top/gtgmrgvhsa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtgqpjlnge.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtlmkciijv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtbsptgshq.html

[F12] CSV 读写
来源：http://hz.vqdsnc.cn/gtvkmovavi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj202588.top/gtuiosrjkr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhongyouzk.top/gtordcutjk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gtkyffbzvf.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtgqchwjxd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtaukgxczk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtmosqxunv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sweek.top/gtrrniguxw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtxjjspdgy.html

================================================================================
来源：http://hz.shangyingyoupin.top/gteemmodvf.html

G. 面向对象
来源：http://hz.xuetiantiany.cn/gtauwzmzep.html

================================================================================
来源：http://hz.jlsjyb.cn/gthokhtjqk.html

[G01] 定义类
来源：http://hz.hnqzz.top/gtpcurtcup.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtitmywyif.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtpyuqvjue.html

JS:   class User {}
来源：http://hz.meibo888.top/gtgrkaskro.html

TS:   class User { name: string = ""; }
来源：http://hz.ppjwa.cn/gtzjpjkqry.html

Java: class User {}
来源：http://hz.xinyue.icu/gtphhsytax.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtvjbjbxpz.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtvfpqdwbj.html

C#:   class User {}
来源：http://hz.haohaochexian.top/gtvovrghmj.html

[G02] 构造函数
来源：http://hz.aibaodan.cn/gtqjarboxb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtvtarehpi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtwpomzuwv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtlilihxnz.html

TS:   constructor(public name: string) {}
来源：http://hz.hongshengwenyu.top/gtqfuixqzt.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtmzkhjuhb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtptcsijxz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtiiijjklz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtagpltwon.html

[G03] 实例属性
来源：http://hz.andypj.xyz/gtmpczzhyy.html

Py:   self.name = "x"
来源：http://hz.feifeiyinyue.top/gtzarjyzta.html

PHP:  public string $name = "x";
来源：http://hz.gotoacloud.top/gtxuzronte.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gttnalsulc.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtgvtydwlg.html

Java: private String name;
来源：http://hz.xylfe.cn/gtwjmakbjr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtkibjpnfb.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gtuufylcqx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yueranfly.top/gtneqikjuv.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gtzdstrrlv.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtxzhesyle.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtavcfhgxq.html

JS:   greet() { return this.name; }
来源：http://hz.xziqi.cn/gtncdzgeof.html

TS:   greet(): string { return this.name; }
来源：http://hz.sysykeji.top/gtfltqvveo.html

Java: String greet() { return name; }
来源：http://hz.ydzc1.top/gtvvoicsgd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtzprswwak.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtvueauimi.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtkxqpelka.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtxiyxukok.html

Py:   class Admin(User): pass
来源：http://hz.bjfxy.top/gtpwbqslcf.html

PHP:  class Admin extends User {}
来源：http://hz.aizwys.cn/gtobegrhrz.html

JS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtdtxxkrpj.html

TS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtpfeqlwus.html

Java: class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtonqcunvj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtawfzgiyf.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gtroguhkei.html

C#:   class Admin : User {}
来源：http://hz.shuidangran.top/gtavtwofky.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtpjxwntue.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtbgukbdsd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtnhpfrybm.html

JS:   greet() { return "admin"; }
来源：http://hz.cheryme.top/gtodaxtpyd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtjxfblggu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtzhihkfpr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtfzksnady.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtuofbguyi.html

C#:   public override string Greet() => "admin";
来源：http://hz.zycfv.cn/gthmraamom.html

[G07] 调用父类方法
来源：http://hz.ivvv.top/gtwauxvlyl.html

Py:   super().greet()
来源：http://hz.yj20258888.top/gtoxlwhffg.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtjczabufu.html

JS:   super.greet();
来源：http://hz.cqqwz.cn/gthyqrznih.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gthvbxeehc.html

Java: super.greet();
来源：http://hz.jianghu66.top/gtjtivinwo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtwbcmcrgi.html

Ruby: super
来源：http://hz.zhaomingkeji.xyz/gtwydbnabo.html

C#:   base.Greet();
来源：http://hz.xingfuxueyuan.xyz/gtkgwjhwvi.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtiymegkmp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cheryme.top/gtmhnrbnjk.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtqilduidy.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtdauynjyc.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtdojwplqb.html

Java: static void f() {}
来源：http://hz.ywan-chungtsiang.top/gtcnqrqbjz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dianchejie.cn/gtukepewkt.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtulmqcmjx.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtvtkbaxik.html

[G09] 接口 / 抽象类
来源：http://hz.andypj.xyz/gtznegvlyn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gttjcojgxf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gthezrtehz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtzwatlqhp.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gthtqzqdua.html


<!-- 参考信息 -->