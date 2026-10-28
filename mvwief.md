代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgfzy.top/gtnymsikcp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gtwxelgfkk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shangyingyoupin.top/gtlnrzlsiy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtibhmlaur.html

[E06] 替换子串
来源：http://hz.xingfuxueyuan.xyz/gtphxsrkkt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtbtxremoc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yongpay.top/gtwryjstbz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtzujxhgcp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtkbvaidyy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtkkyccoqv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cucudq.cn/gtukosdxch.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenlongwang.top/gtobpesuev.html

C#:   s.Replace("a", "b")
来源：http://hz.birdmap.top/gtizwathel.html

[E07] 按分隔符拆分
来源：http://hz.hammf.cn/gtweoybqmv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgufenzy.top/gtkuhgmube.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aizwys.cn/gtmwhpvpvm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fzhhl.top/gtrcypcdfx.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gtgkfxjhlw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.52xcode.cn/gtmwlfvcuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gttweimpsr.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtkjlfnako.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinqigufen.top/gtblusblit.html

[E08] 数组按分隔符合并
来源：http://hz.sxryk.cn/gtfcrcxzqv.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gtcjufzsgz.html

PHP:  implode(",", $items);
来源：http://hz.jiagoushi.top/gtgijeixil.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtrnbillsd.html

TS:   items.join(",")
来源：http://hz.nanxuanxn.top/gticpilpyk.html

Java: String.join(",", items)
来源：http://hz.cqqwz.cn/gtsfrtxmvo.html

Go:   strings.Join(items, ",")
来源：http://hz.jianghu66.top/gtqiexriij.html

Ruby: items.join(",")
来源：http://hz.smart0.xyz/gtnlhuvvea.html

C#:   string.Join(",", items)
来源：http://hz.nwbrower.top/gtxergqkam.html

[E09] 去除所有空白字符
来源：http://hz.meibo888.top/gtkzliqipe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtyjitjqgu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj202588.top/gtogozrlyl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtilrilkaj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtdsnaeblv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ppjwa.cn/gtrstmqxky.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuxming.cn/gtcpixggsq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258.top/gtaicxpjot.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtlvonkmpb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtfpkdecwl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtjqowuknt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtxtgauvar.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtxyysqhze.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtbnjejmhi.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtoebznifn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jianghu66.top/gtwcwobvwf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtdypfkjvf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgfzy.top/gtbsatjdsi.html

[E11] 反转字符串
来源：http://hz.yuanzhike.top/gtxaofhvey.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtavuvuuwr.html

PHP:  strrev($s);
来源：http://hz.ehwqpu.com/gtgofvwvbh.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gthgyqwbau.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtvhsbqrni.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.smart0.xyz/gtkscmfoct.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gtnrjcncgy.html

Ruby: s.reverse
来源：http://hz.birdmap.top/gtguokdtoh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtiymluumv.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gttwaollbk.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtkauwemvm.html

PHP:  substr_count($s, "a");
来源：http://hz.zhongyouzk.top/gtxmemqhvm.html

JS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gtufcrljfz.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtvmevvmee.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gtmujnrglo.html

Go:   strings.Count(s, "a")
来源：http://hz.gzhubu.top/gtonoeyyyb.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtpjhekheh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aibaodan.cn/gtrloluvus.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtkftzsvzl.html

Py:   for ch in s: print(ch)
来源：http://hz.gzhubu.top/gtjrtouazz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ppjwa.cn/gtrvyivays.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtukakydgp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ybcxt.top/gtuyjryvug.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.0kj1m.cn/gtfxupbctz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gtkasjubng.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fengsongda.top/gtghjcsscg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xylfe.cn/gtmmxaeqzd.html

[E14] URL 编码与 Base64
来源：http://hz.haohaochexian.top/gtqrkakjlt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.iojbl.cn/gtfpjuycwd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cashguo.top/gtecljarrf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gthsbbsnda.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258.top/gtmhbainyr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gthawksvgp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gaohongyu789.top/gtvzzemieg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenjidiqi.icu/gtcpqjyawr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtlzaynjwa.html

[E15] HTML 转义 / 反转义
来源：http://hz.yvedp.cn/gtbeoijisk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtcivhxtfi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daria6918.cn/gttsprmdtg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gttejzhkuz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cqqwz.cn/gtszipbavs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhongyouzk.top/gtgrxpyifq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258.top/gtqcmnwvqb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtxmspojwi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtfxmqsunh.html

[E16] 数字千分位
来源：http://hz.nwbrower.top/gtbljopdhz.html

Py:   f"{1234567:,}"
来源：http://hz.cucudq.cn/gtbdeahlpd.html

PHP:  number_format(1234567);
来源：http://hz.jqgufenzy.top/gtdjlwyzbf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gthtlymsmv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtnwdrgctx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtjrqhowse.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.quarkkingdee.top/gtlfogdetd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zdqjudy.top/gtsdlervkg.html

C#:   1234567.ToString("N0")
来源：http://hz.meibo888.top/gtogpkeibi.html

[E17] 首字母大写
来源：http://hz.xuetiantiany.cn/gtpwydhvmt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.iojbl.cn/gtfjpurbev.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ppjwa.cn/gtabqzrwxq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtbscwrmbg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtxypkqyyh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tanke756.top/gtydqvyool.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ywan-chungtsiang.top/gtkurtbvyk.html

Ruby: s.capitalize
来源：http://hz.yvedp.cn/gtkbaslfoz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhengqikj.top/gtvyqbusyx.html

[E18] 模板占位符替换
来源：http://hz.cqqwz.cn/gtmlzdbuhb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtlxjfabbp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gtflismktf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtkuzwqedz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtxtomiock.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.feifeiyinyue.top/gtllewsgzi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guowangkeji.top/gtlupdgmey.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.havefunace.top/gtouqctovw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtcrpsaznk.html

[E19] 多行文本按行拆分
来源：http://hz.nanxinkj.top/gtztbkzbgd.html

Py:   s.splitlines()
来源：http://hz.xylfe.cn/gtsuanxqyf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtvyjsgbpq.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtkrxmqjhc.html

TS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtrrfwurps.html

Java: s.lines().toList()
来源：http://hz.mhx1999.top/gtgkottwtj.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhongyouzk.top/gtijkedqfs.html

Ruby: s.lines
来源：http://hz.quarkkingdee.top/gtgaidtmpe.html

C#:   s.Split('\n')
来源：http://hz.jinqigfzy.top/gtsprucbbd.html

[E20] 判断字符串是否为空
来源：http://hz.zdqjudy.top/gtvbmmhwbe.html

Py:   if not s:
来源：http://hz.xingfuxueyuan.xyz/gtptboyvzx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtkliejyhx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.kuanghao11.cn/gtiohsslil.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtietrnrls.html

Java: if (s.isEmpty()) {}
来源：http://hz.ywan-chungtsiang.top/gtcfgfxare.html

Go:   if s == "" {}
来源：http://hz.gzhubu.top/gtaiwjxqyp.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtuqzhyerv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ywan-chungtsiang.top/gtsymqhkjx.html

[E21] 超长截断加省略号
来源：http://hz.sufxvd.cn/gtohvxywtb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nwbrower.top/gtntoxywxv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtfyjafcdr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtmycdegwq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtubwrihcz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtdamaecbc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgfzy.top/gtnxzwsimz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinghuilouyu.cn/gtxltdhrga.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dianchejie.cn/gtnlzrbazf.html

[E22] 字节长度与字符长度
来源：http://hz.fzhhl.top/gtjxskpdzj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guowangkeji.top/gtciitwdsv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtefrvpdbw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtcdkbarpx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gtxvggotjn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigufen.top/gtntrltdjg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtcaallsju.html

Ruby: s.bytesize;  s.length
来源：http://hz.tian-w.cn/gttrapfozw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtimchcjzv.html

================================================================================
来源：http://hz.yj20258.top/gtvgwjadqh.html

F. 文件与目录
来源：http://hz.zhixingplan.top/gtmelmohjl.html

================================================================================
来源：http://hz.daxiang520.top/gtnrjxbbfx.html

[F01] 读取整个文件
来源：http://hz.chenlongwang.top/gtmtporkup.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtaulgsbov.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtbmtqqcbw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.fengsongda.top/gtvssyxocq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.aizwys.cn/gtxqqucxmg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtqaexkdoy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shzxlz.cn/gtfrwylmxw.html

Ruby: File.read("a.txt")
来源：http://hz.xinyue.icu/gtpphbkqxc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aibaodan.cn/gtxzxosium.html

[F02] 逐行读取文件
来源：http://hz.aibaodan.cn/gtnkoegdsf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtmyjzhoqf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.feifeiyinyue.top/gtttqayjla.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtwmqtiqaz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtorkrkozp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gtiqhpmqsi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yongpay.top/gtnsxmbazb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258888.top/gtknzmgniz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtgegcandv.html

[F03] 写入文件（覆盖）
来源：http://hz.fengsongda.top/gtavpqrkgj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.andypj.xyz/gtkizitcnd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtwwunocbn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtdphgrgso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtotyurpuk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtfiichqlo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangtech.top/gtdnyvmxzu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jyoumei.cn/gtxzazdzhr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gtvtkiuzrf.html

[F04] 追加写入文件
来源：http://hz.sweek.top/gtreijbyyt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jiagoushi.top/gtozfvnoyy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhoulong.xyz/gtijsgejfx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtqynkyaev.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtojdtltvp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jianghu66.top/gtrbklfsrn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtjyslwdim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sweek.top/gtvencjatg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtfwwqbvge.html

[F05] 判断文件或目录是否存在
来源：http://hz.jiagoushi.top/gtylpwcltl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigfzy.top/gtjuddgxao.html

PHP:  file_exists("a.txt");
来源：http://hz.chenzaomai.com/gtyecvqxcw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtrpeoqiqj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtfztsbgnw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtwpnsrtck.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sweek.top/gtltqckdqe.html

Ruby: File.exist?("a.txt")
来源：http://hz.sweek.top/gtaqiemjqg.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtkfqaklgt.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtkxlefcku.html

Py:   os.remove("a.txt")
来源：http://hz.tianlin.xyz/gtxpqeactd.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtlwcivzcq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtajrjxcuq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtfiarqkkc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gthxjbqdcu.html

Go:   os.Remove("a.txt")
来源：http://hz.xinyue.icu/gtlrudsdny.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gtapkpabsj.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtbrtpcfof.html

[F07] 创建目录（含多级）
来源：http://hz.zhongyouzk.top/gtskeqajmr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hfpthk.cn/gtcricwqjz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sxryk.cn/gtudwuwcal.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtvvdktyvd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtfykfeomw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xinyue.icu/gtgmbwirui.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.9152youxi.cn/gtcbhtrngz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jyoumei.cn/gtatnjsxrt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtayqozbts.html

[F08] 遍历目录
来源：http://hz.ybcxt.top/gtfebjwzpc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.andypj.xyz/gtikbpacyv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258.top/gtnazdghki.html

JS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtiwemardo.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gthjwmbgrc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtqollshxe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtijvqvrot.html

Ruby: Dir.children("dir")
来源：http://hz.iojbl.cn/gtetzikqnv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtcspvmboq.html

[F09] 获取文件大小
来源：http://hz.shangyingyoupin.top/gtmxwfbhdv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.c1oappe.top/gtgxwrcmqq.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtdlarlysa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtvjecnrcy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gthxsshamy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtkfhlauet.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtosxwtlal.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtqtikhtjz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhaomingkeji.xyz/gtvrczphrp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuetiantiany.cn/gtajwwuqeq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtsregsvks.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cqqwz.cn/gtivtftgux.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtwlneuxaq.html

TS:   path.extname("a.txt")
来源：http://hz.jinghuilouyu.cn/gtsqmvbevh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtzlfljmlo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtpycoyfsn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtvxwxlfzf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhixingplan.top/gtdemoxvwo.html

[F11] 复制与移动文件
来源：http://hz.yj20258.top/gtsanbdfij.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtmsrjrhdr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jiagoushi.top/gtjqgplzec.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtschujjzd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtzhrsoqqm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.c1oappe.top/gteinijavr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cqqwz.cn/gtjcjdxsup.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtjyogwyum.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shzxlz.cn/gtkvvfipfc.html

[F12] CSV 读写
来源：http://hz.vqdsnc.cn/gtzjzzmzch.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.kuanghao11.cn/gtazmixhdd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtcvyfjkzq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtuuekgiul.html

TS:   // 同上
来源：http://hz.aibaodan.cn/gtrumulzkl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.iojbl.cn/gtapjnoika.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yvedp.cn/gtojnwbtrv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtzqcktytv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gtncnqpdze.html

================================================================================
来源：http://hz.0kj1m.cn/gtsqqwxdyr.html

G. 面向对象
来源：http://hz.jinqigufen.top/gtdctkvhuk.html

================================================================================
来源：http://hz.shuidangran.top/gtcykprlup.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtlbwqesph.html

Py:   class User: pass
来源：http://hz.birdmap.top/gtswejxmjq.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtgvcprwxj.html

JS:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtnxddjzix.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtcexdsxms.html

Java: class User {}
来源：http://hz.yj20258.top/gtybqylhkt.html

Go:   type User struct { Name string }
来源：http://hz.zhoulong.xyz/gtqfrnxxkb.html

Ruby: class User; end
来源：http://hz.ivvv.top/gtkyxpetsg.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtgptmfnmf.html

[G02] 构造函数
来源：http://hz.ydzc1.top/gtpvphszgw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtdkicngrx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtcchpouwm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fengsongda.top/gtphhhgrhd.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtptzufkou.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtrfqagdap.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cqqwz.cn/gtsjezwozv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nwbrower.top/gtwujuclgl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtodovglcn.html

[G03] 实例属性
来源：http://hz.xinyue.icu/gtatddslij.html

Py:   self.name = "x"
来源：http://hz.zhongyouzk.top/gthxckuayl.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtzfhrvhui.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtdnhmvzog.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtrvozxury.html

Java: private String name;
来源：http://hz.daxiang520.top/gtvhmkmfup.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangtech.top/gteapfmxyq.html

Ruby: @name = "x"
来源：http://hz.zhongyouzk.top/gtkpzuippd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cucudq.cn/gtjvgioxzg.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gthmbyqlcu.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtdfahqaqy.html


<!-- 参考信息 -->