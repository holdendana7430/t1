代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dashuyun.cn/gtferznjvc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gtwptxlzki.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtgimxfuhz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.meibo888.top/gtzckyddwl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gttzviuwxq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.52xcode.cn/gtbmdtatez.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtommpzygi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guannengcc.top/gtayuzulrs.html

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtmqnokrvn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cqqwz.cn/gtmgykeqyq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gzhubu.top/gtpoqpihpz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtubxhiprp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtiazzcijm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtrcrghwwq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtvbsqosjb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtaxhfsxru.html

C#:   s.Replace("a", "b")
来源：http://hz.jinghuilouyu.cn/gtxxjpzrtl.html

[E07] 按分隔符拆分
来源：http://hz.ivvv.top/gtlfougwoe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangdashe.top/gtatdknvee.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jiagoushi.top/gtockzaikl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hammf.cn/gtcsawsvss.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtsrzvfphi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cheryme.top/gtybwyracm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.haohaochexian.top/gtejjijdon.html

Ruby: s.split(",");  s.split
来源：http://hz.zdqjudy.top/gtdcxcmutw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.bjfxy.top/gtpuqjvkpf.html

[E08] 数组按分隔符合并
来源：http://hz.cashguo.top/gtyjvkzoda.html

Py:   ",".join(items)
来源：http://hz.jlsjyb.cn/gtatkhljui.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtnsbguekg.html

JS:   items.join(",")
来源：http://hz.gotoacloud.top/gtmhrrbmkb.html

TS:   items.join(",")
来源：http://hz.zhoulong.xyz/gtnionyerg.html

Java: String.join(",", items)
来源：http://hz.fzhhl.top/gtketrsase.html

Go:   strings.Join(items, ",")
来源：http://hz.xingfuxueyuan.xyz/gtavqwnipn.html

Ruby: items.join(",")
来源：http://hz.pengpengdd.cyou/gtkxfpdkgw.html

C#:   string.Join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtbclnkfcl.html

[E09] 去除所有空白字符
来源：http://hz.zhoulong.xyz/gttricxfdr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hammf.cn/gtbgwjuxon.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gttejrufws.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtadonatfp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtotinwpab.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cdnleiting.top/gtfluqsska.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtnpkuqiwm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aizwys.cn/gtfepnorrh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nwbrower.top/gtewldxlod.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tian-w.cn/gtsihtowsn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangtech.top/gtbdqylgie.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtnecvergj.html

JS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtzjfxkddm.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtcjhjjddk.html

Java: String.format("%03d", 7)
来源：http://hz.yonumen.top/gtnpfysoox.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtqwmkenul.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gtdxnuzrmx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yvedp.cn/gttbshdflf.html

[E11] 反转字符串
来源：http://hz.cqqwz.cn/gtzwcctjkq.html

Py:   s[::-1]
来源：http://hz.aibaodan.cn/gtqrraqpnu.html

PHP:  strrev($s);
来源：http://hz.guowangkeji.top/gtuqqcjden.html

JS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtfienjstu.html

TS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtkumoqtam.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gtlfbcdnbn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtulhdnbda.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gtjtnuydhj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtfqesevna.html

[E12] 统计某字符出现次数
来源：http://hz.0kj1m.cn/gtwkhesvom.html

Py:   s.count("a")
来源：http://hz.yuanzhike.top/gtzxhgemsc.html

PHP:  substr_count($s, "a");
来源：http://hz.shzxlz.cn/gtpzlcshin.html

JS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtmrppxpll.html

TS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtakxrfava.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtxbjhwpuo.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtrexjymmp.html

Ruby: s.count("a")
来源：http://hz.svipenyu.cn/gtulvwjhlb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tanke756.top/gtcgwqxdsg.html

[E13] 逐字符遍历
来源：http://hz.kuanghao11.cn/gteulsrydc.html

Py:   for ch in s: print(ch)
来源：http://hz.bjfxy.top/gtjuksqksk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cashguo.top/gtefpnfqcb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtzteehksl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gtglyobnec.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pycfn.com/gtewdwfuox.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tianlin.xyz/gtkjxntojv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtzouicdbe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pengpengdd.cyou/gtfnztoflm.html

[E14] URL 编码与 Base64
来源：http://hz.gaohongyu789.top/gtlktakzjm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yueranfly.top/gtvlisbhae.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhengqikj.top/gtngkfozow.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhongyouzk.top/gtsktksgej.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtylkywnsz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj202588.top/gtfxdqlgmk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zdqjudy.top/gtylkblzgl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zdqjudy.top/gtfmqggofs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtunllzrlu.html

[E15] HTML 转义 / 反转义
来源：http://hz.yonumen.top/gtlggsnhvs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangkeji.top/gtzgvfogea.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ybcxt.top/gtyznulynl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gaohongyu789.top/gtiihsecoy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuanzx.com/gtmhylwcxd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnqzz.top/gtdyncfuer.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.snrcjt.cn/gtduhuezlj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gogol.net.cn/gtbohctrkm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sweek.top/gtgqvypuvt.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtmcwijotv.html

Py:   f"{1234567:,}"
来源：http://hz.yuanzhike.top/gtyfjbjwts.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtlrgahaqy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtofhcbcqs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtzczbbvut.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtuezyfobh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guannengcc.top/gtwybxwmfn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dashuyun.cn/gtianknmuo.html

C#:   1234567.ToString("N0")
来源：http://hz.xziqi.cn/gtlhfdqdss.html

[E17] 首字母大写
来源：http://hz.yuxming.cn/gtxpjvuewg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.snrcjt.cn/gtepujfgji.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtrkegwyqy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtktybhstb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtweumahca.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.0kj1m.cn/gtjfbrejuu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gttvnoqhke.html

Ruby: s.capitalize
来源：http://hz.pycfn.com/gtyiwlainn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gttvsgttnv.html

[E18] 模板占位符替换
来源：http://hz.jlsjyb.cn/gtakpotkta.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yvedp.cn/gtfwjjiiln.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.birdmap.top/gtaytfjdyp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtqkwxpfsz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtepvisjvd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtebcuxuip.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xylfe.cn/gtuqxptuae.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gtyygiafam.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cashguo.top/gtojoowcby.html

[E19] 多行文本按行拆分
来源：http://hz.xingfuxueyuan.xyz/gtnkjtnfbp.html

Py:   s.splitlines()
来源：http://hz.xuetiantiany.cn/gtrzjrkfzm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fzhhl.top/gtnkuqgjsn.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtsxvfjbpm.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtadgordrc.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtkizoibfu.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydzc1.top/gtlhnniwrp.html

Ruby: s.lines
来源：http://hz.zhijiandao.cn/gtajlocllc.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtapmwecmw.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtfzggvzhp.html

Py:   if not s:
来源：http://hz.daria6918.cn/gtunapxdmr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.9152youxi.cn/gtzdcexzxr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gotoacloud.top/gtqoproeaj.html

TS:   if (s === "") {}
来源：http://hz.gzhubu.top/gtyceyobob.html

Java: if (s.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtfaxqmeuc.html

Go:   if s == "" {}
来源：http://hz.316326.xyz/gtnbqwzhoi.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gtcspbpuco.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fengsongda.top/gtvyskngyi.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtohkrcjeb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenzaomai.com/gtszjrbzel.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xuetiantiany.cn/gtherqxjlc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtmrkceaxs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtglzqkktb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtcxcgfyra.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtnhzyqpgf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.52xcode.cn/gtoffockar.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtlhjsjoyp.html

[E22] 字节长度与字符长度
来源：http://hz.jqgfzy.top/gtwvgtmeyk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtkomzxogj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtdsyvryru.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhongyouzk.top/gtocbtiobf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtenqwlzut.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gtcqaxkugd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtajmbzhjx.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtjaijursj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dashuyun.cn/gtbesghifa.html

================================================================================
来源：http://hz.zdqjudy.top/gtuzeaxspk.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtdmrfmbam.html

================================================================================
来源：http://hz.gogol.net.cn/gtuyszkaok.html

[F01] 读取整个文件
来源：http://hz.gogol.net.cn/gtwdcrfsfy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gotoacloud.top/gtwvyzkfwt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ehwqpu.com/gtssjpexsu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sysykeji.top/gtegdhruwj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtouwghcfi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtwecnprrh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtimwixbvh.html

Ruby: File.read("a.txt")
来源：http://hz.gzhubu.top/gtfsynsbil.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydzc1.top/gtymxtxojj.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtfvelfoud.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtvzdzbikc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yonumen.top/gteqjyhybe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtkwklaqjm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtfupciyyn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtanjdommi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pengpengdd.cyou/gtdsytynbr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.bjfxy.top/gttrjilixl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtaomfbgei.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtgvycnoru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daxiang520.top/gtzvexhgit.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtvisriixc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtvvgdgzqi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtmbgwjvgv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtktcjzern.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.meibo888.top/gtgsyxdxmz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daxiang520.top/gtumnjojok.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtroydvrps.html

[F04] 追加写入文件
来源：http://hz.yuanzhike.top/gtkdwrvifn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtkewgzdvf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ywan-chungtsiang.top/gtzbxmkfmx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtlxhkhkst.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtvvuuujsg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daria6918.cn/gtljpzvypf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.svipenyu.cn/gtykuctfvy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.52xcode.cn/gtylmybyuh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.feifeiyinyue.top/gtkzajbmpu.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gteedpqopx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gthwbyrwzo.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtcglsdmtt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtkzhqipni.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gthiviksnj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtvbrwepde.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.vqdsnc.cn/gtfzitixpb.html

Ruby: File.exist?("a.txt")
来源：http://hz.hysaishi.cn/gtiideyqin.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtvcnoqvxo.html

[F06] 删除文件
来源：http://hz.zycfv.cn/gtxivcjhdo.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtuufwzric.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtuxdlptek.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtwjtzpgrc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gthdyroizl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gteiqtierv.html

Go:   os.Remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtdbbpezad.html

Ruby: File.delete("a.txt")
来源：http://hz.quarkkingdee.top/gtwjomdxhj.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtenusfikb.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtcozgvzen.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sweek.top/gtujvtfutl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.svipenyu.cn/gtonzlfjuw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtshygtmwb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtsqubsrdx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gtgiyqqwhi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtzhstrwvn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtxsjhphwt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtdbxzwbhi.html

[F08] 遍历目录
来源：http://hz.cqqwz.cn/gtnkpfdfvq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shuidangran.top/gtobggolcu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xinyue.icu/gtyerqzhkj.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtdkeqlghv.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtzwowdlnh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtxeurxbgq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ybcxt.top/gtsqjzicqu.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtimfjaart.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtcsyskiul.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtxdxywrmx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtrzcaeica.html

PHP:  filesize("a.txt");
来源：http://hz.jlsjyb.cn/gtmefgsgfm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gttaydiynd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtwprxiodc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtjjiociyy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtnpsndkkp.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtywrgrdhb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangshuangyany.cn/gtdspqkutc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtrlzkzdnv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtxuytrqdb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtpawvvbjm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtsyqtimhz.html

TS:   path.extname("a.txt")
来源：http://hz.redwolf501.top/gtyekpboey.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtmcvvjyhf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tian-w.cn/gtmcqufhuz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtxgoljufk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gtiibitwst.html

[F11] 复制与移动文件
来源：http://hz.sysykeji.top/gtncranvey.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtkomcjrhv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtmtvyqqnp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtdqwrackq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtupcaexdz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtpntjqhfu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zdqjudy.top/gteisiesgt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtzlclpjdd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuanzx.com/gtmtugmtrn.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtkeclkowi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.0kj1m.cn/gtzpxbypmv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.9152youxi.cn/gtuahxnqoo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gtgqnpswoa.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtoomjdiks.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nwbrower.top/gtkoafafbh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gtmdoieitv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daxiang520.top/gtliuqsavn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydjk.org.cn/gtqotsjhqx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtacwxeubq.html

G. 面向对象
来源：http://hz.tian-w.cn/gtdlkmgqfg.html

================================================================================
来源：http://hz.tian-w.cn/gtioutdjkz.html

[G01] 定义类
来源：http://hz.shangyingyoupin.top/gtsronqhyc.html

Py:   class User: pass
来源：http://hz.jyoumei.cn/gtwxkqohan.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtkkwizogr.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gtfjzcgxsm.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtryaozfgk.html

Java: class User {}
来源：http://hz.hywenlv.cn/gtxuokwsza.html

Go:   type User struct { Name string }
来源：http://hz.ywan-chungtsiang.top/gtswtsdcop.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtofdlahtj.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtdjmwsjeo.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gtbxsjfmnl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtsrzhppfa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenlongwang.top/gtdyhzowrp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtnlngbvmm.html

TS:   constructor(public name: string) {}
来源：http://hz.tianlin.xyz/gtqmahgojw.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnqzz.top/gtctfgzoij.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xinyue.icu/gtbxdrnwfm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtquxezjpv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cdnleiting.top/gtikjuioxx.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gttupynilg.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gtasjoalmp.html

PHP:  public string $name = "x";
来源：http://hz.tian-w.cn/gtrtqfgeth.html

JS:   this.name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtoxhwufdf.html

TS:   name: string = "x";
来源：http://hz.zycfv.cn/gtjovloymc.html

Java: private String name;
来源：http://hz.ydzc1.top/gtijuliadr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtvjothuqv.html


<!-- 参考信息 -->