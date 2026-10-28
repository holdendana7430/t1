代发 wailian999

[E06] 替换子串
来源：http://hz.yuxming.cn/gtrfcusgua.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtuvaxqfoz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.316326.xyz/gtqetuqllh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gthgzruomc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtveocktow.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtwsydccae.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtimqfzlpr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sysykeji.top/gtgyghtfvt.html

C#:   s.Replace("a", "b")
来源：http://hz.jinyuanbaomall.cn/gthfexgyvm.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtjxbuwdpj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gtpkaojurw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj20258888.top/gtwjfaewgp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinyuanbaomall.cn/gthnfpsadu.html

TS:   s.split(",")
来源：http://hz.shuidangran.top/gtskwxriza.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtrufrbrkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yanxiufei.cn/gthddzltto.html

Ruby: s.split(",");  s.split
来源：http://hz.iojbl.cn/gtsaititbq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhaomingkeji.xyz/gtvbsdupxh.html

[E08] 数组按分隔符合并
来源：http://hz.vqdsnc.cn/gtmfjvpofp.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtoxogtayk.html

PHP:  implode(",", $items);
来源：http://hz.tian-w.cn/gtymuvypaz.html

JS:   items.join(",")
来源：http://hz.zhengqikj.top/gtwhteznun.html

TS:   items.join(",")
来源：http://hz.yangfankeji.com/gtvrthxooa.html

Java: String.join(",", items)
来源：http://hz.gaohongyu789.top/gtmjlxbvwt.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtgrmjkbug.html

Ruby: items.join(",")
来源：http://hz.vqdsnc.cn/gtwiohvbks.html

C#:   string.Join(",", items)
来源：http://hz.fengsongda.top/gtyvklnprz.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtumfylfmj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gttzodnufy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenlongwang.top/gtradznxtd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtfezxvuqo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtvqdnfyft.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtnepuermg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtfsrmbpdi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gtshlwcbpb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtexauimnh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dashuyun.cn/gtgjyzeqhx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.fengsongda.top/gtrvtkmvso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cqqwz.cn/gtnogdhjxb.html

JS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gtnmytttlr.html

TS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtvypcqimu.html

Java: String.format("%03d", 7)
来源：http://hz.hnxiangtu.top/gttzwzicws.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtzgpdillj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gtyvvjwlwj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtabvmphhk.html

[E11] 反转字符串
来源：http://hz.vqdsnc.cn/gtiqkjmjey.html

Py:   s[::-1]
来源：http://hz.pycfn.com/gtmkxejbxd.html

PHP:  strrev($s);
来源：http://hz.xinyue.icu/gtsankbmor.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtdrsdpnkl.html

TS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtjiflrmxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtyazwdmad.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinyuanbaomall.cn/gtkzanlvqw.html

Ruby: s.reverse
来源：http://hz.jianghu66.top/gtfgjnmkai.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gtqhntdzuo.html

[E12] 统计某字符出现次数
来源：http://hz.redwolf501.top/gtkzrnaoqm.html

Py:   s.count("a")
来源：http://hz.cashguo.top/gtfitbrvqy.html

PHP:  substr_count($s, "a");
来源：http://hz.zhixingplan.top/gtfpxoipqb.html

JS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtwyqdvwnh.html

TS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gtjuhjohtk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtgirzeqci.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gttjondzpw.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtajschnyq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gzhubu.top/gtshildjkz.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtvsvkqepo.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gtqxeloceh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenjidiqi.icu/gtdxrvrawn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtrzbahxbe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtzdtcrjku.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gtfofyhlej.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shzxlz.cn/gtvgswugva.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xylfe.cn/gtwzmmdeiz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hammf.cn/gtahztqpzm.html

[E14] URL 编码与 Base64
来源：http://hz.jinyuanbaomall.cn/gtkaecupab.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gtundgbamf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.quarkkingdee.top/gtqnozdlpp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.birdmap.top/gtakhxkolo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenlongwang.top/gtkeuqczod.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sysykeji.top/gtbhapkmqy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhijiandao.cn/gtfpgqjpno.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.haohaochexian.top/gtwznfneic.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ybcxt.top/gtrfpybokb.html

[E15] HTML 转义 / 反转义
来源：http://hz.xingfuxueyuan.xyz/gtkuivcfcw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.kuanghao11.cn/gtdpxljsih.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtdcsubegw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xziqi.cn/gtvvibljqp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.0kj1m.cn/gtwdtbqtea.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtyntexcrc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ehwqpu.com/gtahdxcvpx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtdyweimhq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tanke756.top/gtbryztnmc.html

[E16] 数字千分位
来源：http://hz.havefunace.top/gtgbeqhwbd.html

Py:   f"{1234567:,}"
来源：http://hz.hnxiangtu.top/gtrqxopcjf.html

PHP:  number_format(1234567);
来源：http://hz.jinqigufen.top/gtmnpsqzqn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtxhfcmtku.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtqbjvqdkr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gtmryphwhy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.52xcode.cn/gtvsppqfhk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtqyuzwxdu.html

C#:   1234567.ToString("N0")
来源：http://hz.aizwys.cn/gtgtwigybk.html

[E17] 首字母大写
来源：http://hz.aizwys.cn/gtrccwvjvc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xziqi.cn/gtoljaqaaf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydzc1.top/gtmqowkovm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtkhfilhee.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtdzbmqhbm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj20258888.top/gtnkkaeyvb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fzhhl.top/gtpsbrxpyz.html

Ruby: s.capitalize
来源：http://hz.daxiang520.top/gtyzvpddqa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtbixhpchk.html

[E18] 模板占位符替换
来源：http://hz.tian-w.cn/gtoflzqkxw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sufxvd.cn/gtspafgysg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhoulong.xyz/gtyiklvqds.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtirrtxcoy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hongshengwenyu.top/gttpmpknnm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtjkrgkjoc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhixingplan.top/gtxwmhjfry.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtoskqtvpv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhixingplan.top/gthrijffns.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtwkmxdcsm.html

Py:   s.splitlines()
来源：http://hz.hfpthk.cn/gtbgfwirbr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.kuanghao11.cn/gthglvdrzn.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gthhttqyhu.html

TS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtulxadvnn.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtdfifngzu.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtbmyonzkz.html

Ruby: s.lines
来源：http://hz.pengpengdd.cyou/gtyrvmjcal.html

C#:   s.Split('\n')
来源：http://hz.gotoacloud.top/gtqzihvaos.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gteieawmox.html

Py:   if not s:
来源：http://hz.ywan-chungtsiang.top/gtvnwwfdgl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxinkj.top/gtstzdwmou.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtujpbloxv.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtsvbchdlv.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnqzz.top/gthebmhmww.html

Go:   if s == "" {}
来源：http://hz.cdnleiting.top/gtdersuyki.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gterhfxhvh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ehwqpu.com/gtobyejqid.html

[E21] 超长截断加省略号
来源：http://hz.hysaishi.cn/gtyiebhyam.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gthjvwlfxd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenjidiqi.icu/gtlvtfjrjz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtqtnitzex.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtzalxtrhr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtjmihrmvg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigfzy.top/gtnxrhccco.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guannengcc.top/gtbxyqyhbj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yueranfly.top/gtqzramdfr.html

[E22] 字节长度与字符长度
来源：http://hz.xinyue.icu/gtthnjpulj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtvkrwrkmt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtxxunjuod.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtqdimjwdj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtbzfitorx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gtzvuvlieq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gteeuahrgo.html

Ruby: s.bytesize;  s.length
来源：http://hz.yonumen.top/gtlshgnjyx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sysykeji.top/gtxcezprcp.html

================================================================================
来源：http://hz.yongpay.top/gtozpfwtwh.html

F. 文件与目录
来源：http://hz.gzhubu.top/gtsqpvqmpe.html

================================================================================
来源：http://hz.yonumen.top/gtnznevgoo.html

[F01] 读取整个文件
来源：http://hz.xuanzx.com/gtgrhdarqu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj202588.top/gtznfpcsqd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yongpay.top/gtodgjtauc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gtlpegujkp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtsfcvijea.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtxxepfaje.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gttgjsqczt.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtfzlmkirp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenzaomai.com/gterwbfxej.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtkytktvoj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fengsongda.top/gtcfudbfqk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtjyeupjqu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtphcgjkcy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtcbqrvzvu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtxefrhvje.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fengsongda.top/gtptrshmpt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtanvzmary.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aizwys.cn/gtfojnsqkp.html

[F03] 写入文件（覆盖）
来源：http://hz.tanke756.top/gtsdotpnzq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxinkj.top/gtrgqcgqeu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sweek.top/gtudbybkye.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtyhjuyfta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtokzwhkku.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtzlarblqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gogol.net.cn/gtziopphwd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.snrcjt.cn/gtmmfdxnyk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fengsongda.top/gtsphjdyyl.html

[F04] 追加写入文件
来源：http://hz.shzxlz.cn/gtkgajflkw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtuzovxpxe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtqornnebp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtwokulpqs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtqpicqywu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhiwuduotai.top/gtsamxhbba.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gteysahrfk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigufen.top/gtvdayoqpa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.quarkkingdee.top/gthzsnndsq.html

[F05] 判断文件或目录是否存在
来源：http://hz.dianchejie.cn/gtnmricnci.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtlfezaqzw.html

PHP:  file_exists("a.txt");
来源：http://hz.zdqjudy.top/gtlejspyky.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtoueldnpn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtlpslvadk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtlxcorbmw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gtrjcdywqm.html

Ruby: File.exist?("a.txt")
来源：http://hz.gogol.net.cn/gttyycildn.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtlnmschnn.html

[F06] 删除文件
来源：http://hz.nanxuanxn.top/gtootxtcqd.html

Py:   os.remove("a.txt")
来源：http://hz.yueranfly.top/gthvcbxeny.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtliywtoww.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtmrhlmhbq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtxdfyhgve.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtgtvmetlk.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gteufvdqnx.html

Ruby: File.delete("a.txt")
来源：http://hz.zdqjudy.top/gtggjwfdru.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtaagafpzp.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtbvdftjed.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ehwqpu.com/gtaizwpbao.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtnyyemkvd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtgnbajfru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtcjuvfcjb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtqllnqlnj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtgyxolswl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gtzabxubvp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zycfv.cn/gtaeycriyq.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtosovpvfq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hysaishi.cn/gtvkbcxiil.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtpzlqrsgu.html

JS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtqroedpxt.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtuzbpufsc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtwzkfmlly.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtjrjppvrj.html

Ruby: Dir.children("dir")
来源：http://hz.aibaodan.cn/gtjlfjpaes.html

C#:   Directory.GetFiles("dir")
来源：http://hz.0kj1m.cn/gtilvmlfwj.html

[F09] 获取文件大小
来源：http://hz.tianlin.xyz/gtyfmrwybz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtfbwbxajj.html

PHP:  filesize("a.txt");
来源：http://hz.ydjk.org.cn/gtpmyzmzma.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtqicdaltg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtoelrvrgr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtwqiijujr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangdashe.top/gtzjfgeorc.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gtorxzusek.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnqzz.top/gtqhhurpxt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtllvawqau.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtqzxgpsiw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hysaishi.cn/gtglcdvbtx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtcohmnias.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtozkqkmjv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yueranfly.top/gtetwiwbpl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guowangkeji.top/gtmqhivpfx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtryanpvqp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtxbxjcopq.html

[F11] 复制与移动文件
来源：http://hz.fengsongda.top/gtecqliaov.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtveezymlx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtjkymxmar.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtdmkoucya.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtyozsbdpi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gttsraopjd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangkeji.top/gtjxkkoknc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtlzgpwqvq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cqqwz.cn/gtkmtrcpsn.html

[F12] CSV 读写
来源：http://hz.ybcxt.top/gtubyevqhh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gtqsixbmnp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jiagoushi.top/gtkxdwclvq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.52xcode.cn/gtqrjryuat.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtkcuvhdgg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gaohongyu789.top/gtqvuzfljr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gtbjuwnqis.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gtjthhyenx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtfhbkmoln.html

================================================================================
来源：http://hz.haohaochexian.top/gtsyajwcwv.html

G. 面向对象
来源：http://hz.dianchejie.cn/gtpbnagjoo.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbaiynshg.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtzwqsiyjm.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtcrltxbwo.html

PHP:  class User {}
来源：http://hz.pengpengdd.cyou/gtyzylplge.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtyzpxuttk.html

TS:   class User { name: string = ""; }
来源：http://hz.hammf.cn/gtajygqrgs.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gtnewdrhfq.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtohoabrkt.html

Ruby: class User; end
来源：http://hz.zhaomingkeji.xyz/gthfqnwcct.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtfywtdbbk.html

[G02] 构造函数
来源：http://hz.0kj1m.cn/gtagdpuegm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangkeji.top/gteehyzpny.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenlongwang.top/gtopmyrlqa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gthidqdnwj.html

TS:   constructor(public name: string) {}
来源：http://hz.cucudq.cn/gtcjryhntk.html

Java: User(String name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtpqpjntbv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtxpmjvoyg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shuidangran.top/gtytlrcpht.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gogol.net.cn/gtrqghxfri.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtvqwomfos.html

Py:   self.name = "x"
来源：http://hz.smart0.xyz/gtibeepupj.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtqjkgasux.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtcjyrcsjz.html

TS:   name: string = "x";
来源：http://hz.hammf.cn/gtbbeboqhv.html

Java: private String name;
来源：http://hz.ywan-chungtsiang.top/gtsozpmoxe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnxiangtu.top/gtehyyuvqr.html

Ruby: @name = "x"
来源：http://hz.tanke756.top/gtckktlfvu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhixingplan.top/gtyqtepchr.html

[G04] 定义方法
来源：http://hz.quarkkingdee.top/gtcourqjzg.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtghshtamx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gteahboduz.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtixyzcciu.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtjlfqpeqd.html

Java: String greet() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtjeaezetw.html


<!-- 参考信息 -->