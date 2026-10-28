代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ywan-chungtsiang.top/gtgovwftlh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jiagoushi.top/gttlhgkbgt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ppjwa.cn/gtpvfhbyfc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigfzy.top/gtrbsbpfny.html

[E06] 替换子串
来源：http://hz.gogol.net.cn/gtyowzgsnk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ppjwa.cn/gtospjledc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cqqwz.cn/gtznjgbsmk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtuiqstqrg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtuctvkrma.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtruohvsox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.andypj.xyz/gtbkbrthzq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtujidhhio.html

C#:   s.Replace("a", "b")
来源：http://hz.chenjidiqi.icu/gtoaxxkhjp.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gtzswjfvhp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtadhfqsbq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.iojbl.cn/gtugpdaxpz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.guowangkeji.top/gtjtytiafj.html

TS:   s.split(",")
来源：http://hz.hongshengwenyu.top/gtqcxacblu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.52xcode.cn/gtgmlgxevl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cheryme.top/gtzddprtzy.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtncyrkzsi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daxiang520.top/gtcpdktcxv.html

[E08] 数组按分隔符合并
来源：http://hz.wangshuangyany.cn/gtlqwaprgm.html

Py:   ",".join(items)
来源：http://hz.hnqzz.top/gtjbuweetr.html

PHP:  implode(",", $items);
来源：http://hz.gotoacloud.top/gtjkeodhif.html

JS:   items.join(",")
来源：http://hz.tianlin.xyz/gtrvphzvkq.html

TS:   items.join(",")
来源：http://hz.nanxinkj.top/gtawoalmtv.html

Java: String.join(",", items)
来源：http://hz.kuanghao11.cn/gtuezekutr.html

Go:   strings.Join(items, ",")
来源：http://hz.andypj.xyz/gtnkejddpi.html

Ruby: items.join(",")
来源：http://hz.xziqi.cn/gtibvqttgy.html

C#:   string.Join(",", items)
来源：http://hz.xuetiantiany.cn/gtfgiavpzb.html

[E09] 去除所有空白字符
来源：http://hz.zhiwuduotai.top/gtqgwyqrnl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtytufhasw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jyoumei.cn/gtgsyfglrg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtixvckqcv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gthfxbtavg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shangyingyoupin.top/gtemavjpbp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtfqysmhjj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tianlin.xyz/gtlcchdogy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sysykeji.top/gtgphfdguf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxinkj.top/gtotijprsk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tian-w.cn/gtqvpwapdi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtqznueerl.html

JS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtvlxgzxqs.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtahtagjho.html

Java: String.format("%03d", 7)
来源：http://hz.zhengqikj.top/gtpynckdwr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtkjnzsqpq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuxming.cn/gtyqwqrpjl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtcculhpty.html

[E11] 反转字符串
来源：http://hz.birdmap.top/gtyogjljqv.html

Py:   s[::-1]
来源：http://hz.ppjwa.cn/gtwnfylaby.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtothstdhh.html

JS:   [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtqbyewbfb.html

TS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtqzwgkeis.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtibaluktj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtwiltjxvh.html

Ruby: s.reverse
来源：http://hz.hnxiangtu.top/gtrohrfytp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.mhx1999.top/gtsggcokyx.html

[E12] 统计某字符出现次数
来源：http://hz.gzhubu.top/gtkbfxyrys.html

Py:   s.count("a")
来源：http://hz.guannengcc.top/gtagblhwvs.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtzyttzwph.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtrckkatpq.html

TS:   s.split("a").length - 1
来源：http://hz.cheryme.top/gtfuckrjeg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtgifixddu.html

Go:   strings.Count(s, "a")
来源：http://hz.0kj1m.cn/gtqbgjyejk.html

Ruby: s.count("a")
来源：http://hz.cashguo.top/gtjkcxssdz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gtuirpucuw.html

[E13] 逐字符遍历
来源：http://hz.nanxinkj.top/gtvipgexdn.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtuqojrfuj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aibaodan.cn/gtwbhphrza.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gttxhczvom.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtvyvatyxt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtqavrkvoq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jyoumei.cn/gtgwwszaag.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sufxvd.cn/gtzdyaaysu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gtpxxtqypq.html

[E14] URL 编码与 Base64
来源：http://hz.vqdsnc.cn/gtlmfcomvc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.iojbl.cn/gtuqpuqkxm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dianchejie.cn/gttqeznecc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sufxvd.cn/gtrqxbnxdi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pycfn.com/gtdlpurpoh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gtgluamsgj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.smart0.xyz/gtwdozzofi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gotoacloud.top/gtyuwgsdru.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258888.top/gtbpgrgnnj.html

[E15] HTML 转义 / 反转义
来源：http://hz.vqdsnc.cn/gtvdpjdbdo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtyyqtpuet.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtlgyzxbkh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigufen.top/gtfxudjntc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ybcxt.top/gtgdtfjlyp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuanzx.com/gtdawaqere.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.smart0.xyz/gtkyppsyxl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yongpay.top/gttigxqywk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.iojbl.cn/gtibkcrspr.html

[E16] 数字千分位
来源：http://hz.ywan-chungtsiang.top/gtdmetiofy.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtjoocxjxo.html

PHP:  number_format(1234567);
来源：http://hz.chenzaomai.com/gtonoieouh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtyjprkxuw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gthyezupck.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258.top/gtdbjnadya.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cheryme.top/gtxzyabpcl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.kuanghao11.cn/gtfndqvfdc.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gttxbnixts.html

[E17] 首字母大写
来源：http://hz.xinyue.icu/gtqqahgvhi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gtqcbiodai.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtljyrqtok.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gtvbaumvaw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtbbjmdyia.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sufxvd.cn/gtmnolrbvq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtyhchppca.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gtopyaaosp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nwbrower.top/gthjwgmdvv.html

[E18] 模板占位符替换
来源：http://hz.fengsongda.top/gtqxxgsdyo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sweek.top/gtmlbtybot.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenjidiqi.icu/gtpsywnkcj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtdmntuvxe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtukrtysyo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgfzy.top/gtxudlhmbk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gtdjkrswbk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtgxngjkgl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtslrnstbe.html

[E19] 多行文本按行拆分
来源：http://hz.gaohongyu789.top/gtfwkxknts.html

Py:   s.splitlines()
来源：http://hz.chenzaomai.com/gtiaqwquej.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangshuangyany.cn/gtotdgzjae.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtcdgzeoqs.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtxfobhexf.html

Java: s.lines().toList()
来源：http://hz.sufxvd.cn/gtwxjeqkxt.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtfjegekku.html

Ruby: s.lines
来源：http://hz.fengsongda.top/gtmleuddov.html

C#:   s.Split('\n')
来源：http://hz.yuxming.cn/gtuxfoenwt.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtzbotnhha.html

Py:   if not s:
来源：http://hz.yongpay.top/gtlsmdclul.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hywenlv.cn/gthfjivkyw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.c1oappe.top/gtnnsjykbi.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtygignmzh.html

Java: if (s.isEmpty()) {}
来源：http://hz.nwbrower.top/gtndwhurwz.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gtnoaxxjvv.html

Ruby: if s.empty?
来源：http://hz.ybcxt.top/gthwurpzze.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gttvarswmi.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtsiskvzdr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.bjfxy.top/gtbmqijrzm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hfpthk.cn/gtqexpyezg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtmpmrvzlw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtenxnabxx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtkrchfsev.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guannengcc.top/gtmhnkxneu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gaohongyu789.top/gtosplifxu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fzhhl.top/gtffirebks.html

[E22] 字节长度与字符长度
来源：http://hz.yj202588.top/gtfiiwvlxt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhongyouzk.top/gtunytxqhe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yvedp.cn/gttpphygpt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtutmxvimx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtanwepoiv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gtxocbwnfr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgufenzy.top/gtnewyjbiy.html

Ruby: s.bytesize;  s.length
来源：http://hz.redwolf501.top/gthlfbhhwx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.mhx1999.top/gtaoxtqpqx.html

================================================================================
来源：http://hz.shzxlz.cn/gtgagtsmyo.html

F. 文件与目录
来源：http://hz.mhx1999.top/gtmesreunt.html

================================================================================
来源：http://hz.zhengqikj.top/gtwrazdfji.html

[F01] 读取整个文件
来源：http://hz.chenjidiqi.icu/gtaxmedpms.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtdhexkkgf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gthjgpqlgj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenzaomai.com/gtbkgssoqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fzhhl.top/gtflrxlxel.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtjuqwkuxy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigfzy.top/gtzarstvbj.html

Ruby: File.read("a.txt")
来源：http://hz.jiagoushi.top/gthevflgaa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.redwolf501.top/gtijondznw.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtziadohqp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtheeqplde.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sxryk.cn/gtmhegbfbe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gthauqaiqq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtuxytoqjn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gthfohatys.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xylfe.cn/gtpdljfzld.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtdnmjrjym.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258.top/gtaiflxfna.html

[F03] 写入文件（覆盖）
来源：http://hz.hnxiangtu.top/gtgqptdnaj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hfpthk.cn/gtbugdpgcz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.bjfxy.top/gtciledpsd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuetiantiany.cn/gtxyifqgbi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtdajfehoj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jianghu66.top/gtygfoxmvo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtlmwlrrlq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yvedp.cn/gtocyvtmbs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtxxekoalq.html

[F04] 追加写入文件
来源：http://hz.pycfn.com/gtwkmfzvtj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gtfwqzgwch.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sysykeji.top/gtolktnqpc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtfxaqrtqk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtkyttyctp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gtnevjnayd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sweek.top/gtaemcahfy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtrxjfkoza.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gtpxkyfwhr.html

[F05] 判断文件或目录是否存在
来源：http://hz.yonumen.top/gthjgfelae.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tianlin.xyz/gtbhlzwdci.html

PHP:  file_exists("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtidxanryf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtjsxvtzgr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtnfczzqux.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtsqkxnsez.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxuanxn.top/gtqalyvxav.html

Ruby: File.exist?("a.txt")
来源：http://hz.316326.xyz/gtejxfaqyv.html

C#:   File.Exists("a.txt")
来源：http://hz.ydzc1.top/gtypshmhgw.html

[F06] 删除文件
来源：http://hz.gaohongyu789.top/gtotevpqmw.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtrqvvavbl.html

PHP:  unlink("a.txt");
来源：http://hz.jianghu66.top/gtnhmalykh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtbhqjpyvd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtfwewzmpt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtpgkhlaxp.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtjjngmata.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmqsqfzwn.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtvewobiyg.html

[F07] 创建目录（含多级）
来源：http://hz.tianlin.xyz/gtkzirngyx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtkekgoexv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.birdmap.top/gtfpjijycx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtosqslusa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtcyryseuw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daria6918.cn/gtpplumixl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigufen.top/gtyyoskhcb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtfswwietr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigufen.top/gtoqguqmgq.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtnfixdcra.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhaomingkeji.xyz/gtmimtbvvi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtbktmfpnq.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtopkyvuzw.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtugspjrmj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gttycihytc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hammf.cn/gtihkijybx.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtdwmoajzp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgufenzy.top/gtwmxqrodd.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtjcrmzlyk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gtetaadfed.html

PHP:  filesize("a.txt");
来源：http://hz.mhx1999.top/gtcxbbwtjs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtzcrlekys.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtzkhbcgjx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtjpphjcty.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtnwjmnnkp.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtvyridyzh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtniaelilv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtkrfmzprl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtibhmxwix.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtuumcknme.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtisqtgptx.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtkqswfbnf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnxiangtu.top/gtdblgeoum.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zycfv.cn/gtrffqmkcu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtgnyflbsa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.havefunace.top/gtmmkurbra.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtlwoxxpjz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtzthcfaix.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj202588.top/gtscbdtpsn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtqfpjglok.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtszrogeti.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtkmrmpzty.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtqsmrkqij.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtlczvudxk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinyuanbaomall.cn/gtzsfyyunh.html

[F12] CSV 读写
来源：http://hz.cqqwz.cn/gtmxzhbasr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtzekwoeml.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigufen.top/gtbequjcop.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shuidangran.top/gtgrlmpbdq.html

TS:   // 同上
来源：http://hz.hfpthk.cn/gtlrjwydnt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pengpengdd.cyou/gtiiyjhwju.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gtbpbfbcib.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtewzlxpla.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.0kj1m.cn/gtuhraifgk.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtllnaevxv.html

G. 面向对象
来源：http://hz.cqqwz.cn/gtvensjpjv.html

================================================================================
来源：http://hz.dashuyun.cn/gtgogeajfl.html

[G01] 定义类
来源：http://hz.0kj1m.cn/gtsonmeiui.html

Py:   class User: pass
来源：http://hz.jqgufenzy.top/gtltuxhcje.html

PHP:  class User {}
来源：http://hz.zhoulong.xyz/gtfhatsbow.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtgbottuho.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtefostyix.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtwboyfspr.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtnkhwjdvf.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gtquuugorr.html

C#:   class User {}
来源：http://hz.xuanzx.com/gtrjukxfyu.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtblkqyuwk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtbqoyevty.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xylfe.cn/gtfpqykmfr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sysykeji.top/gtnfnmrnmt.html

TS:   constructor(public name: string) {}
来源：http://hz.hnxiangtu.top/gtkrybwesc.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtpejfreyi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gzhubu.top/gtlpoihwta.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gtlpxnaxeo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cucudq.cn/gtmujhpjbn.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtzidvqmnm.html

Py:   self.name = "x"
来源：http://hz.yonumen.top/gtcwrghaqv.html

PHP:  public string $name = "x";
来源：http://hz.ppjwa.cn/gtcfanjmkn.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtkemqwclb.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtwovidcuw.html

Java: private String name;
来源：http://hz.zycfv.cn/gtturcfvqf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtvorqylbp.html

Ruby: @name = "x"
来源：http://hz.ydzc1.top/gtcpwnrunh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cucudq.cn/gtzukugfbz.html

[G04] 定义方法
来源：http://hz.yanxiufei.cn/gtvkiyzaee.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtpnawkyzk.html


<!-- 参考信息 -->