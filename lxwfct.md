代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gtegnsorfl.html

[E07] 按分隔符拆分
来源：http://hz.cdnleiting.top/gtfhxmmpst.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gtvmysiaaz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jlsjyb.cn/gtwggazehm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtkhrvsjxx.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gtutgbsxex.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.birdmap.top/gtusgmwndk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hnxiangtu.top/gtnpagwgcc.html

Ruby: s.split(",");  s.split
来源：http://hz.316326.xyz/gtowuejipo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.mhx1999.top/gtvpyfojkm.html

[E08] 数组按分隔符合并
来源：http://hz.gogol.net.cn/gtezcsuyol.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtacwakqol.html

PHP:  implode(",", $items);
来源：http://hz.guannengcc.top/gtgqwkwidu.html

JS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gttqzavcgs.html

TS:   items.join(",")
来源：http://hz.hnqzz.top/gtjkfhrloa.html

Java: String.join(",", items)
来源：http://hz.zhiwuduotai.top/gthblmrybz.html

Go:   strings.Join(items, ",")
来源：http://hz.c1oappe.top/gtbaavwhsk.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtkfjfyzhw.html

C#:   string.Join(",", items)
来源：http://hz.zhijiandao.cn/gtjfriqsxy.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gtoibgclua.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.feifeiyinyue.top/gtoydrrsda.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtuaclpdaq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sufxvd.cn/gtfthsunbt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtllbbcuik.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pengpengdd.cyou/gtqkfgrwmj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fzhhl.top/gtqjgriajz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.quarkkingdee.top/gteasyqyiq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zdqjudy.top/gtlpmalfwi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258888.top/gtgcdinpyl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hfpthk.cn/gtzrbeqdhg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cqqwz.cn/gtpjavcfue.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtgpmgaxpz.html

TS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtyyqzbwdj.html

Java: String.format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtmbrtrbqj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnxiangtu.top/gtvaulerxf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tanke756.top/gtqkwqarir.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtqiljaauk.html

[E11] 反转字符串
来源：http://hz.bjfxy.top/gtcegqbqiz.html

Py:   s[::-1]
来源：http://hz.wangdashe.top/gtntoycsua.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtmfvficgj.html

JS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gteqrupxnj.html

TS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtduzmtyqg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cucudq.cn/gtxwqzuzxo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxuanxn.top/gtyygtcewt.html

Ruby: s.reverse
来源：http://hz.jlsjyb.cn/gtklvyghbr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtehujevst.html

[E12] 统计某字符出现次数
来源：http://hz.iojbl.cn/gttfacqqhj.html

Py:   s.count("a")
来源：http://hz.havefunace.top/gtxhojorcp.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtatwbnwuk.html

JS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtqbvqsjvn.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtuxakxrrv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigfzy.top/gtwecirkui.html

Go:   strings.Count(s, "a")
来源：http://hz.daxiang520.top/gtvjiuqcta.html

Ruby: s.count("a")
来源：http://hz.yj20258888.top/gtblaphfyy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shzxlz.cn/gthmtaearl.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtcctcvnkl.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gthlbiovni.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shangyingyoupin.top/gtqmnwlgpl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtgechdaps.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtgiqgoviz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtduuzfsbf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shangyingyoupin.top/gtjcbcjran.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cucudq.cn/gtpzduimwv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtpralwblr.html

[E14] URL 编码与 Base64
来源：http://hz.jyoumei.cn/gthtdqbffv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtmghbmofr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhijiandao.cn/gtoynjynvn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gtldwjakrh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zycfv.cn/gtwzyqipqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhengqikj.top/gtqreuzvet.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gtyactyxvs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtdbbobprv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tian-w.cn/gtuobgogxk.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtuszkbdst.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhengqikj.top/gtvpwmnpwg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.9152youxi.cn/gtiiiezkgi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtymesnutu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pycfn.com/gtwagujyce.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.0kj1m.cn/gttncrpiuc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtooefqhvz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuetiantiany.cn/gtwnpcvtrg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.haohaochexian.top/gtjgbncmge.html

[E16] 数字千分位
来源：http://hz.zdqjudy.top/gtnjzsjxty.html

Py:   f"{1234567:,}"
来源：http://hz.haohaochexian.top/gtpwwbpdam.html

PHP:  number_format(1234567);
来源：http://hz.jinqigufen.top/gttookmkmd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtamcmrnba.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtoqacifli.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtcptpepre.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ehwqpu.com/gtmyaheqnx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hfpthk.cn/gtkklnofmo.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258888.top/gtpvelbxkq.html

[E17] 首字母大写
来源：http://hz.yj202588.top/gtwkddhnwi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ivvv.top/gtmafftepy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sxryk.cn/gtwnbekrwe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtsypiezxy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtznjsyhzn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.snrcjt.cn/gtwgjjwlyl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nwbrower.top/gtdrsnojpi.html

Ruby: s.capitalize
来源：http://hz.andypj.xyz/gtvtttzmzq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cucudq.cn/gtbjvdodqa.html

[E18] 模板占位符替换
来源：http://hz.hfpthk.cn/gtvoeiuoky.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tianlin.xyz/gtudrhiygn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tianlin.xyz/gtykrmnitk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtwqcedflz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtkhqokzlv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.snrcjt.cn/gthzdxgdcc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtmtezvlnq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuetiantiany.cn/gtuxvfafnw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.vqdsnc.cn/gtpgyqzlbu.html

[E19] 多行文本按行拆分
来源：http://hz.cdnleiting.top/gtsxcysylf.html

Py:   s.splitlines()
来源：http://hz.hysaishi.cn/gtfhwcffbm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtkquwrclw.html

JS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtcxtmocuc.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtykigrygk.html

Java: s.lines().toList()
来源：http://hz.jianghu66.top/gtpjrpvtec.html

Go:   strings.Split(s, "\n")
来源：http://hz.tanke756.top/gtwvdtphzr.html

Ruby: s.lines
来源：http://hz.ppjwa.cn/gtjjwkenhk.html

C#:   s.Split('\n')
来源：http://hz.jqgfzy.top/gtdpgbheva.html

[E20] 判断字符串是否为空
来源：http://hz.nanxinkj.top/gtkhyjeanb.html

Py:   if not s:
来源：http://hz.chenlongwang.top/gtthgymfvw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gttodclvqg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtpaytdmwe.html

TS:   if (s === "") {}
来源：http://hz.hammf.cn/gttlyiiuxa.html

Java: if (s.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtzwvfzief.html

Go:   if s == "" {}
来源：http://hz.316326.xyz/gtgtcdwvfq.html

Ruby: if s.empty?
来源：http://hz.jlsjyb.cn/gtijgblvct.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtpqbdsgjw.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gtknyzwufe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinyuanbaomall.cn/gtchhxajjz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhijiandao.cn/gtkmzracro.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtyrmztqxb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtqfzulonb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtmwofihhk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guowangkeji.top/gtkgjoavnl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtrwyenzub.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yangfankeji.com/gtsdbwxxrf.html

[E22] 字节长度与字符长度
来源：http://hz.zhixingplan.top/gtnzmxiide.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtenpjsoei.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gttwgnjzos.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtzrzzgfjk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtfogtgrmb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydzc1.top/gtyukjdqfb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.c1oappe.top/gtgxwxtoqe.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gtvfhqaeyx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gtotadyclt.html

================================================================================
来源：http://hz.daxiang520.top/gtznvmvywg.html

F. 文件与目录
来源：http://hz.xylfe.cn/gtjkeetqgz.html

================================================================================
来源：http://hz.zdqjudy.top/gtvabiipqh.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtjdspnmga.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtdsojhjth.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gthxqowrkd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hammf.cn/gtxlvuxfwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cqqwz.cn/gtkbeewgno.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtftxqozdc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtdtiugund.html

Ruby: File.read("a.txt")
来源：http://hz.nwbrower.top/gtyvsstkny.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydjk.org.cn/gtozqrphco.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtacxcvacx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtsdmrvckj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhixingplan.top/gtzrtughpx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtfctdxtst.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gthgomwock.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gttcthuxuh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuetiantiany.cn/gtevizarbh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtusztsawj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shzxlz.cn/gtxzrgkynu.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258888.top/gtebvibllv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangshuangyany.cn/gtckjypvqn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sxryk.cn/gtswrwgmdn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtfpdpwqcw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtbgbtgecn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtvvkmmmfp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sufxvd.cn/gtwmvqvxeh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenlongwang.top/gtobgcsxhn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ivvv.top/gtetrctars.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtovlokcpb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pycfn.com/gthhhwcyff.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuanzx.com/gtqkcoadiv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtthcwlojt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtnuetrsrq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aizwys.cn/gtzcsrtvng.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtdjeefcii.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gtatgrjyhu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258.top/gtimxkdugr.html

[F05] 判断文件或目录是否存在
来源：http://hz.zycfv.cn/gthktvoxdx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydjk.org.cn/gtiqwxytmd.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtywcnfeqt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtxjhzzqsq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtwqhjowds.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtrepyyipa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtcjjscfon.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtkuizzype.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtdluidfvi.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtjiqoeoyr.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtobdghqjf.html

PHP:  unlink("a.txt");
来源：http://hz.jianghu66.top/gtjemmcnkh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtxexdbcgh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtzralfcqd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtxxzxcusa.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtxnjtjqcj.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtuzmyrbey.html

C#:   File.Delete("a.txt");
来源：http://hz.snrcjt.cn/gtydrwgirh.html

[F07] 创建目录（含多级）
来源：http://hz.gotoacloud.top/gtednledbv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtlmopvmio.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jyoumei.cn/gteyllarnd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtrqviscqq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtrucydqrs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jiagoushi.top/gtcfhlnwvd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtpsiakawg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ivvv.top/gtsrnkoqzx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gaohongyu789.top/gtfgahfkfq.html

[F08] 遍历目录
来源：http://hz.nanxuanxn.top/gtmqcmzwmt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cdnleiting.top/gthbhdzgwy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangshuangyany.cn/gtwcbkooli.html

JS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gtcnwozuyu.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtudbnytcq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtzgivrsdk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtzgtdozeq.html

Ruby: Dir.children("dir")
来源：http://hz.ybcxt.top/gtiqekdjlp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtdtaujnfc.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gticazgjol.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtxmqhkhep.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigfzy.top/gtmmlafpld.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtiwbofodr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtotberexw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtggbkbecx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtzradktmf.html

Ruby: File.size("a.txt")
来源：http://hz.9152youxi.cn/gtlcytazqv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtyqeiwdoc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnqzz.top/gtgbewwsve.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtvrsuqfmq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gtmqiilqyy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtiojmwbbd.html

TS:   path.extname("a.txt")
来源：http://hz.yueranfly.top/gtepjqmfae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gtbefdnati.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtsgedixtf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtkqveqilx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.kuanghao11.cn/gthlkjylwo.html

[F11] 复制与移动文件
来源：http://hz.sweek.top/gtahksitvn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtuwplwebm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtlwivztnx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtbstuhwmj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gthovxckvt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guowangkeji.top/gtvutpfnep.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtnfvwlsxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtynanczsc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gtaumffbkk.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtfyyhomzt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.havefunace.top/gtwqihazhg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gtbpokptmf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtdiahpnwl.html

TS:   // 同上
来源：http://hz.jyoumei.cn/gtwvjdsnvv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gtexqvaqvi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cashguo.top/gtbukchsms.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cheryme.top/gttmlkqioc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gtunkvduvj.html

================================================================================
来源：http://hz.cheryme.top/gtkwoqsbit.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtkzhbkdnf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtdztziyct.html

[G01] 定义类
来源：http://hz.havefunace.top/gtkviqkllh.html

Py:   class User: pass
来源：http://hz.chenjidiqi.icu/gtshbxzmle.html

PHP:  class User {}
来源：http://hz.gzhubu.top/gtjgvyimxs.html

JS:   class User {}
来源：http://hz.yongpay.top/gtjqysakku.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtqzwpvpsx.html

Java: class User {}
来源：http://hz.hnxiangtu.top/gtdtcdtyyq.html

Go:   type User struct { Name string }
来源：http://hz.shzxlz.cn/gtqwhfgsfk.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtsamcldxo.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtzgsmvqet.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtriorqnfq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtqkixfyhn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhiwuduotai.top/gttynfvzhm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtdfpnzgvn.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtsshogikc.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gtlonizyif.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhijiandao.cn/gttjbbyncm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gtlqmainlx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shangyingyoupin.top/gtuleovsom.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtwvwkschw.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtldnsshvm.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtbejbvozp.html

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtljhvohcl.html

TS:   name: string = "x";
来源：http://hz.cqqwz.cn/gtqqwlfzdv.html

Java: private String name;
来源：http://hz.9152youxi.cn/gtprpikmle.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gteuulizrp.html

Ruby: @name = "x"
来源：http://hz.guannengcc.top/gtvrpuvwhc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangdashe.top/gtyjetwsfl.html

[G04] 定义方法
来源：http://hz.xziqi.cn/gtjwrphvep.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtkpijvwri.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtrhrclapz.html

JS:   greet() { return this.name; }
来源：http://hz.xuanzx.com/gtwuxttvfs.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtzdwgcfcr.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtefiwxplj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtldegubqy.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gtorxvqufd.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtqogmhiqy.html

[G05] 继承
来源：http://hz.yanxiufei.cn/gtbpexizwr.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtjulfhrak.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258.top/gthiesluai.html

JS:   class Admin extends User {}
来源：http://hz.birdmap.top/gthzuewgvp.html

TS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtzwxgxigx.html


<!-- 参考信息 -->