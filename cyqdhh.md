代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hywenlv.cn/gtyebxzzhn.html

TS:   s.slice(1, 4)
来源：http://hz.chenlongwang.top/gtithwsyqe.html

Java: s.substring(1, 4)
来源：http://hz.yuxming.cn/gtfwvwszxg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.wangdashe.top/gtqwklucsc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtdcbnondo.html

C#:   s.Substring(1, 3)
来源：http://hz.sweek.top/gtzghyjppp.html

[E04] 查找子串位置
来源：http://hz.dashuyun.cn/gtbyezqucz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtbdcodtse.html

PHP:  strpos($s, "x");
来源：http://hz.yueranfly.top/gtmzcjhott.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.feifeiyinyue.top/gthkveefsw.html

TS:   s.indexOf("x")
来源：http://hz.zhixingplan.top/gtathdrjlm.html

Java: s.indexOf("x")
来源：http://hz.meibo888.top/gtogrniilx.html

Go:   strings.Index(s, "x")
来源：http://hz.tanke756.top/gtqvafrcvs.html

Ruby: s.index("x")
来源：http://hz.xuetiantiany.cn/gtbkyusfum.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtrnnbinns.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnqzz.top/gtyhpxxedr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhixingplan.top/gtshzssiko.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guowangkeji.top/gtmpkipiuz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtslicikin.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nwbrower.top/gtcqllqnls.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtjlioibfd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.52xcode.cn/gtjmznzxuf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hammf.cn/gtkbccygny.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fzhhl.top/gtgtblnbud.html

[E06] 替换子串
来源：http://hz.jinqigufen.top/gtflesyhqh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ppjwa.cn/gtercnruhh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuetiantiany.cn/gtauohlxfv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtstwmnfui.html

TS:   s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtmhtihqos.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtjzfzfuth.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cdnleiting.top/gtqddlalhs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtvakegswn.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gtndqwvhca.html

[E07] 按分隔符拆分
来源：http://hz.sxryk.cn/gtwzwfayks.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.birdmap.top/gtqbnmlleh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.316326.xyz/gtxomsfztq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gthehrksul.html

TS:   s.split(",")
来源：http://hz.yvedp.cn/gtjnmfwybp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sweek.top/gtcpravzlb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xingfuxueyuan.xyz/gtiilgtxwg.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtmvfvkylx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jyoumei.cn/gtthmrhjfm.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtotegddic.html

Py:   ",".join(items)
来源：http://hz.bjfxy.top/gtdknhsgrb.html

PHP:  implode(",", $items);
来源：http://hz.xuetiantiany.cn/gtrnhiajto.html

JS:   items.join(",")
来源：http://hz.316326.xyz/gtmbvbrekj.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtbqxqjjmz.html

Java: String.join(",", items)
来源：http://hz.ydjk.org.cn/gtdldqqtdn.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gttdemlpdc.html

Ruby: items.join(",")
来源：http://hz.pycfn.com/gtgjydldnl.html

C#:   string.Join(",", items)
来源：http://hz.tian-w.cn/gtjihhwgyy.html

[E09] 去除所有空白字符
来源：http://hz.wangshuangyany.cn/gtdfflnyog.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hywenlv.cn/gtmfjxiwwd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydzc1.top/gteqiatbcw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtmxmuenxv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gthueablki.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangdashe.top/gtrtjmdrks.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.c1oappe.top/gtzvxbtayb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigufen.top/gttzowuehy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gtvlinkynk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cashguo.top/gtberqekey.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtuyfcjnki.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ppjwa.cn/gtmslrwqhz.html

JS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtmfjbepej.html

TS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtmedhrrgu.html

Java: String.format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtsuqogden.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.havefunace.top/gtnkgjakxx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zdqjudy.top/gtaxvymfjv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtwagbnbgo.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtgztcofjl.html

Py:   s[::-1]
来源：http://hz.ydjk.org.cn/gtpsledcpe.html

PHP:  strrev($s);
来源：http://hz.cheryme.top/gtsszfccgx.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtimxtiedm.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtpxqmcyym.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.feifeiyinyue.top/gtxmlpzeqp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.havefunace.top/gtqjpaasrd.html

Ruby: s.reverse
来源：http://hz.tianlin.xyz/gtdttxumkk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtytxarmdz.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gthhwcfzvf.html

Py:   s.count("a")
来源：http://hz.yj20258888.top/gtdqzlswml.html

PHP:  substr_count($s, "a");
来源：http://hz.kuanghao11.cn/gtmuwznqev.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtbnzspyid.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtgeguzduf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenlongwang.top/gtyypihroc.html

Go:   strings.Count(s, "a")
来源：http://hz.hongshengwenyu.top/gtqpcauilz.html

Ruby: s.count("a")
来源：http://hz.birdmap.top/gtawaoiiwz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yvedp.cn/gtzuhryeqq.html

[E13] 逐字符遍历
来源：http://hz.jiagoushi.top/gthbpkhrck.html

Py:   for ch in s: print(ch)
来源：http://hz.zhiwuduotai.top/gtuuazegpx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jianghu66.top/gtzrrnawwd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtfecldsfm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cashguo.top/gteuvaingn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.iojbl.cn/gtnjdtmmqm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yvedp.cn/gtgotbtoza.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtbhdsyilv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtbsobqqtb.html

[E14] URL 编码与 Base64
来源：http://hz.cashguo.top/gtrehtqfio.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.9152youxi.cn/gttlrpxgme.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.havefunace.top/gttwvxobme.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenzaomai.com/gtkyumceyy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gtlhbanmyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jlsjyb.cn/gtfwmlbodq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.iojbl.cn/gtdwisbnuy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cucudq.cn/gtyfpjdldn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.haohaochexian.top/gtqnwoulfy.html

[E15] HTML 转义 / 反转义
来源：http://hz.xziqi.cn/gtabbvehja.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xziqi.cn/gtnlulfuli.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.smart0.xyz/gtwpdhtmhc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.svipenyu.cn/gtocasfywf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuanzhike.top/gtmgadidyg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yonumen.top/gtznbquxvn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinghuilouyu.cn/gtdtmpgccu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gtrdhkdaed.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtdeqklrxy.html

[E16] 数字千分位
来源：http://hz.gzhubu.top/gtoyewqupd.html

Py:   f"{1234567:,}"
来源：http://hz.yueranfly.top/gttshgsqbf.html

PHP:  number_format(1234567);
来源：http://hz.guowangkeji.top/gtfdxfbkmz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtewvsllko.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtformbuba.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtfpuomvnd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gtjvkthzhb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtyeqqwebq.html

C#:   1234567.ToString("N0")
来源：http://hz.xuetiantiany.cn/gtcnxwhtcf.html

[E17] 首字母大写
来源：http://hz.sysykeji.top/gtsumviogh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtlxbhvlks.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinghuilouyu.cn/gtlyspyban.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuxming.cn/gtiuqghjpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtalppmzkp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xingfuxueyuan.xyz/gthxudgeys.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cdnleiting.top/gtjkparker.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtxhyrqubq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gttxgwjjfj.html

[E18] 模板占位符替换
来源：http://hz.pengpengdd.cyou/gtczhdxdbj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtggjqdbsh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gteiokfeug.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtyoynbuse.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtzwkvoine.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gtcmcxtbvc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gttmrguppp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cqqwz.cn/gtqndffbdc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtvhrrtozh.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gttfjltmsg.html

Py:   s.splitlines()
来源：http://hz.wangdashe.top/gtsftybgmj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.kuanghao11.cn/gtcihbebrx.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtiwdkrdbf.html

TS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtzhmkosqi.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtvtvffnjq.html

Go:   strings.Split(s, "\n")
来源：http://hz.meibo888.top/gthljnjpqn.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtqzxxpsvp.html

C#:   s.Split('\n')
来源：http://hz.ivvv.top/gtngykfqhd.html

[E20] 判断字符串是否为空
来源：http://hz.pengpengdd.cyou/gtdykwevmk.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtrhewlsyi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxuanxn.top/gtnlvdwbcs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigfzy.top/gthpkhiohu.html

TS:   if (s === "") {}
来源：http://hz.gotoacloud.top/gtietoxeri.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gthqlzxjcp.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtlxseslxz.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtaekcgxhv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shangyingyoupin.top/gttwdlfupa.html

[E21] 超长截断加省略号
来源：http://hz.cqqwz.cn/gtddtqwezt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.vqdsnc.cn/gtnfqattzg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.pengpengdd.cyou/gtodjsrhdo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtwjhndqhq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gttfpanwou.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtzejpodfo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtrjcudjaz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.9152youxi.cn/gtslvfhzja.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhongyouzk.top/gtsfkoszat.html

[E22] 字节长度与字符长度
来源：http://hz.mhx1999.top/gtlaipwbre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydzc1.top/gtsvrnakmj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtswyyvfyy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtozufuauh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtrmcxvneb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gtqehpexhx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtrosyyhdh.html

Ruby: s.bytesize;  s.length
来源：http://hz.mhx1999.top/gtgklhiytv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtlolbgnze.html

================================================================================
来源：http://hz.fengsongda.top/gtyqkluqio.html

F. 文件与目录
来源：http://hz.xylfe.cn/gtildwzydw.html

================================================================================
来源：http://hz.hfpthk.cn/gtpwywcygk.html

[F01] 读取整个文件
来源：http://hz.gzhubu.top/gtszzejrke.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.andypj.xyz/gtlkxvzonf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fzhhl.top/gtgqatrune.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtxojlxfix.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tian-w.cn/gtqfimudep.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtkejsqnbk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtsbeyoefc.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gtjwzzcuue.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sufxvd.cn/gtxdtckyyu.html

[F02] 逐行读取文件
来源：http://hz.yongpay.top/gtiaufkieu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhengqikj.top/gtlbisubiq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xylfe.cn/gtngeyyipo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gttklokwjn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtlwrkvdwm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtqqcqkdyy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtusolzhxo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daxiang520.top/gtdzieoqau.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtekjzhuop.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtozzoztzr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gtqalbmuzb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gttjfidzzc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtzfofqwol.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gtnrjnvlvr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sxryk.cn/gtacnmaibr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtmypqcqpt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cheryme.top/gtuhqnlsdn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.316326.xyz/gtgbeeakht.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtvzdbktnf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ivvv.top/gtcisgxrqp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.vqdsnc.cn/gtlsakztpt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtywcfwflg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtbammhfbp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtotucunac.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ydzc1.top/gtiqdvfavq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigfzy.top/gtvfrqyuka.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtdrhfdmaf.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtddtiajxh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.svipenyu.cn/gtsmbpzbgu.html

PHP:  file_exists("a.txt");
来源：http://hz.yongpay.top/gtmhgsidzt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtqcuzgvyg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtwajxthjj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtithwwxsr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuanzx.com/gturafqwyz.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtjqetnydb.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtywiypvbu.html

[F06] 删除文件
来源：http://hz.ivvv.top/gtchzvzwfd.html

Py:   os.remove("a.txt")
来源：http://hz.sxryk.cn/gtvtvrbsmp.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtxqdzqgde.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtnojhajrp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtlhmivmtx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtykimqguf.html

Go:   os.Remove("a.txt")
来源：http://hz.andypj.xyz/gtwuxgamvc.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gtfdbcprln.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gtbwdpxzoy.html

[F07] 创建目录（含多级）
来源：http://hz.xuetiantiany.cn/gttnmgrdwt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gthufvswov.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.quarkkingdee.top/gtvrylpxlo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtdebacluk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtxirxbeyj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtzrbzlwga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gtyqzayiyp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jianghu66.top/gtoumuwpeh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtymagvmfs.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gtjsgdawew.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zycfv.cn/gtuohvqtsq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj202588.top/gtpjkyfxdn.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtxbxrbptv.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtvcgbgbbp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtofiruvmq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtvquhyexg.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangkeji.top/gtshkciepu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhijiandao.cn/gtsrozwgxa.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtnvplphpl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.52xcode.cn/gtigojmjlf.html

PHP:  filesize("a.txt");
来源：http://hz.zhiwuduotai.top/gtlzxlvepv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtsmtsjgej.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gtygoegmoh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtezrqhxeg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtidukgjde.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gtnnstqwdl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtgoslflko.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.haohaochexian.top/gteavuaffy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtuylapqza.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yangfankeji.com/gtmibriotn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtzzobjawo.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtmxiebrju.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jlsjyb.cn/gtionzrpgf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yvedp.cn/gtztflalpa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtobxvlbty.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtncvvbgzg.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtzljpndfj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtknthgffh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgufenzy.top/gtyrkplbza.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtgtazflsa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtbfmssdkb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gticdvycny.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gzhubu.top/gtkprwzhuu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtufwinwhl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtpfsetpyo.html

[F12] CSV 读写
来源：http://hz.hnxiangtu.top/gtwizeulth.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aizwys.cn/gtrkqkqsxu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhaomingkeji.xyz/gtvpnintfh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtmexxauel.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtfozjyjij.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.kuanghao11.cn/gteugjxttp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dianchejie.cn/gtxsepvxea.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nwbrower.top/gtneobvehn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtaiiulfuy.html

================================================================================
来源：http://hz.xylfe.cn/gtjqontawv.html

G. 面向对象
来源：http://hz.sysykeji.top/gttlxbnetj.html

================================================================================
来源：http://hz.0kj1m.cn/gtrsdxsase.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtkrqlnshs.html

Py:   class User: pass
来源：http://hz.shanyushiyangtech.top/gtuzfesqux.html

PHP:  class User {}
来源：http://hz.jinqigfzy.top/gtavafwgvt.html

JS:   class User {}
来源：http://hz.hnqzz.top/gtbnrwmand.html

TS:   class User { name: string = ""; }
来源：http://hz.jlsjyb.cn/gtlihglfbm.html

Java: class User {}
来源：http://hz.yj202588.top/gtdubbzoah.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtvcioffvb.html

Ruby: class User; end
来源：http://hz.wangdashe.top/gtkzupsynp.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtdjuntwqb.html


<!-- 参考信息 -->