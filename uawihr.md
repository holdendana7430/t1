代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtwllxdcll.html

[E03] 截取子串
来源：http://hz.zhongyouzk.top/gtspdnkzqs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sxryk.cn/gtlcfkbnry.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gotoacloud.top/gtqpcsyjue.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.meibo888.top/gtvsflerxc.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtvspkdxas.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtkkhtdfyw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.bjfxy.top/gtjjnryohx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.pengpengdd.cyou/gtyefrtbvu.html

C#:   s.Substring(1, 3)
来源：http://hz.9152youxi.cn/gthbchfnmt.html

[E04] 查找子串位置
来源：http://hz.pengpengdd.cyou/gtydxrtpxv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xziqi.cn/gtphmpgsxq.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtrwgmpwxf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xingfuxueyuan.xyz/gtogguyvpd.html

TS:   s.indexOf("x")
来源：http://hz.andypj.xyz/gtpqzrzzdz.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtihrxnisz.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxuanxn.top/gtjamydlrd.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gtjsmjssnd.html

C#:   s.IndexOf("x")
来源：http://hz.jlsjyb.cn/gtqnmijdvn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gtzjmggdbb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yvedp.cn/gtgqvgzikg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhixingplan.top/gtkwfbvrng.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtjzsqqmvn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.kuanghao11.cn/gtgnczoddn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnxiangtu.top/gthdpoahrv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tianlin.xyz/gtakslsmkv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dashuyun.cn/gtolcnxvcd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtdgbphjiq.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gtbhyfhgmn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sxryk.cn/gtaeqbnbif.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.vqdsnc.cn/gtqsomjyja.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtrxgdkcid.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtadstujxw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtjoizatal.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtldgdvfhj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.meibo888.top/gtpekjdcvf.html

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gtywrpvlll.html

[E07] 按分隔符拆分
来源：http://hz.jinqigufen.top/gtalhwlona.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtlokemlkq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gtsvnjmane.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gtczimkmkr.html

TS:   s.split(",")
来源：http://hz.gogol.net.cn/gtbxgzhhtr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tian-w.cn/gtxxzxhuye.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.birdmap.top/gtwkqturar.html

Ruby: s.split(",");  s.split
来源：http://hz.xinyue.icu/gtufeompuv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuanzhike.top/gtrfrqhdnc.html

[E08] 数组按分隔符合并
来源：http://hz.fengsongda.top/gtwyswjdcp.html

Py:   ",".join(items)
来源：http://hz.zhiwuduotai.top/gtpxlnniaa.html

PHP:  implode(",", $items);
来源：http://hz.dashuyun.cn/gtkyqpvrzo.html

JS:   items.join(",")
来源：http://hz.cashguo.top/gtovdkbdos.html

TS:   items.join(",")
来源：http://hz.andypj.xyz/gtuwjvwthg.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtdhrmtuid.html

Go:   strings.Join(items, ",")
来源：http://hz.fzhhl.top/gtzeuubwqp.html

Ruby: items.join(",")
来源：http://hz.zhengqikj.top/gtiprbhoez.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangtech.top/gtpguatlxq.html

[E09] 去除所有空白字符
来源：http://hz.xuanzx.com/gtetzfxpii.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxuanxn.top/gtvlsvcvot.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenlongwang.top/gthbjbudyi.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtjtxriqyb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtxphxmojl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.dianchejie.cn/gtzommguvl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.redwolf501.top/gtaijntsky.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtosiuyhqy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gtbzfegoix.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tianlin.xyz/gtambznkns.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtfkztrdmi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.0kj1m.cn/gtgabmcuwh.html

JS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtowiostqj.html

TS:   "7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtbdtpvaac.html

Java: String.format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtkgxujzae.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gttbsmqhvi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.haohaochexian.top/gttkygdsfk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dashuyun.cn/gtxjxswopu.html

[E11] 反转字符串
来源：http://hz.cheryme.top/gtdyfycevw.html

Py:   s[::-1]
来源：http://hz.zhongyouzk.top/gtngxezwtm.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtvmmljaxb.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtefqvfodp.html

TS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtksppmhqq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.smart0.xyz/gtuicdqmzl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtksofsevh.html

Ruby: s.reverse
来源：http://hz.jinghuilouyu.cn/gtgfdwnlbm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtreyxmwlt.html

[E12] 统计某字符出现次数
来源：http://hz.chenlongwang.top/gtfgveebjl.html

Py:   s.count("a")
来源：http://hz.hnqzz.top/gtnsafxtfm.html

PHP:  substr_count($s, "a");
来源：http://hz.ydjk.org.cn/gtpzvmbedi.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtmzthfmlt.html

TS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtgbdczjex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangdashe.top/gtcfasqlng.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gtzwgfauuf.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtfscpnnfu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtvrimjbrl.html

[E13] 逐字符遍历
来源：http://hz.shzxlz.cn/gtqqyagkkp.html

Py:   for ch in s: print(ch)
来源：http://hz.xylfe.cn/gthrwvuawu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xingfuxueyuan.xyz/gtirqjddyn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtzzyqnqas.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gticjfsavr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jiagoushi.top/gttmehmhgb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xinyue.icu/gtjekchoxb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenlongwang.top/gtyxhzdwcv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yanxiufei.cn/gtepaiiiwg.html

[E14] URL 编码与 Base64
来源：http://hz.jinyuanbaomall.cn/gtuengpmbu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhiwuduotai.top/gtkcpfuvmk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xziqi.cn/gtjwkxsusw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtbccvipbf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtwinskfxc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hammf.cn/gtbnjzswrg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gtsnkgcdvx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yangfankeji.com/gtsfeenhzf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgufenzy.top/gtbnnpxhxx.html

[E15] HTML 转义 / 反转义
来源：http://hz.fzhhl.top/gtjpmewdjw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.havefunace.top/gtxketujlh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gteedrnygd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.feifeiyinyue.top/gtceyvrsbh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtlnjylysg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtwawlszgk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtonatoapc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shuidangran.top/gtlajutpsg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnxiangtu.top/gtuexjmluy.html

[E16] 数字千分位
来源：http://hz.xingfuxueyuan.xyz/gtncczewkr.html

Py:   f"{1234567:,}"
来源：http://hz.wangdashe.top/gtdwoywqtb.html

PHP:  number_format(1234567);
来源：http://hz.gaohongyu789.top/gtbvudmcwl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtecljroyq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gthcfffkfi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtpxvafyoy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtihqncjeg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daxiang520.top/gtqvxgcryf.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtlovlatqw.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gtjvopvtbd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tian-w.cn/gtvzbllzdm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nwbrower.top/gtytuepxrg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtfyrhjeth.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtnzapnvab.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.andypj.xyz/gtdoltoqrm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cashguo.top/gtmlynezfk.html

Ruby: s.capitalize
来源：http://hz.yuanzhike.top/gtwfwugdaf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zycfv.cn/gthpndxofx.html

[E18] 模板占位符替换
来源：http://hz.c1oappe.top/gtvypyhjal.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenlongwang.top/gtzrcqsklu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gtpecenybs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtssxgnqdp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtaptrknfq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtminnwfkc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtojxdndkr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtkhbjtaxl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtlkryjodf.html

[E19] 多行文本按行拆分
来源：http://hz.sweek.top/gtnfhdniuh.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangtech.top/gttfgovagk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhijiandao.cn/gtxpiojqjx.html

JS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtiwiiiiiu.html

TS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtlibrrchy.html

Java: s.lines().toList()
来源：http://hz.yuanzhike.top/gtagugbuhn.html

Go:   strings.Split(s, "\n")
来源：http://hz.cheryme.top/gtprcprpmh.html

Ruby: s.lines
来源：http://hz.cashguo.top/gtfuvguesc.html

C#:   s.Split('\n')
来源：http://hz.cashguo.top/gtrmstnsxa.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangkeji.top/gtshjshpjt.html

Py:   if not s:
来源：http://hz.shanyushiyangtech.top/gtaotcptsk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtkyvebvet.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hongshengwenyu.top/gtudsddyff.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gtajmsilaq.html

Java: if (s.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtfywdqvag.html

Go:   if s == "" {}
来源：http://hz.sysykeji.top/gtnlircqdv.html

Ruby: if s.empty?
来源：http://hz.xziqi.cn/gtgdndahvq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhixingplan.top/gtwkautkyc.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtgugxsrsb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hywenlv.cn/gtlvwouueo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtvzbvivym.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtwkpfhsgw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtvfgfmhos.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtxsgmsfdv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yanxiufei.cn/gtxpsrlepc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fzhhl.top/gtbaqgmouu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhengqikj.top/gtednpdohs.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtjxuavrgv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtypqkfgde.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtqoldiuwu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtkgsatrxj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtxvdlddjz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtgfjuiffu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtfrliqafi.html

Ruby: s.bytesize;  s.length
来源：http://hz.ywan-chungtsiang.top/gtdmwqfhbi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.smart0.xyz/gtbkwuokhr.html

================================================================================
来源：http://hz.guannengcc.top/gtikhgztpm.html

F. 文件与目录
来源：http://hz.gotoacloud.top/gtxgmfuyqd.html

================================================================================
来源：http://hz.sweek.top/gtyraoyykc.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtntgilxub.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.guowangkeji.top/gtolsxneyo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cqqwz.cn/gtlhstgsnx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhongyouzk.top/gtglumravi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxuanxn.top/gtfyhpjioy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gthdprfici.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtltwrsmdg.html

Ruby: File.read("a.txt")
来源：http://hz.meibo888.top/gtqqfuvzfe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtatbycxkv.html

[F02] 逐行读取文件
来源：http://hz.xingfuxueyuan.xyz/gthqelbkmr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gogol.net.cn/gtqnkxybtu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pycfn.com/gtehwhjpej.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtutagxyrb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtjkyzyltd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtjsunagaa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gotoacloud.top/gthkbupsoz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.havefunace.top/gtrlqgsxja.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ywan-chungtsiang.top/gtgppouzlz.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gtyjcgtlet.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zycfv.cn/gtjznovunu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtwwrcykoe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtnwuloqes.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtkukymhnq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtctvfaull.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gteoadmvye.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xziqi.cn/gtrzaxlndj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtlxgnwfjo.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtmmopjonp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ivvv.top/gtjgyxekfy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258888.top/gtchyplmyg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtuvkobkou.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtadmhcfzq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtkkywttfc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sufxvd.cn/gtasvixiuh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtyirxzahq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtbfcjvsvz.html

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtusfqhcft.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gotoacloud.top/gtnodxjlkp.html

PHP:  file_exists("a.txt");
来源：http://hz.jianghu66.top/gtkgclpivj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtakmxfuxd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gtgnwdrvff.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtqyldjwpr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gtvtudjtay.html

Ruby: File.exist?("a.txt")
来源：http://hz.tianlin.xyz/gtyykodoug.html

C#:   File.Exists("a.txt")
来源：http://hz.vqdsnc.cn/gtttikqkzd.html

[F06] 删除文件
来源：http://hz.9152youxi.cn/gtgdxxporx.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gtmxrwvdvc.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gtfzxqclut.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtjjzusjnf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gttbijivbq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtyuqfthis.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtoilloasn.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtlpiwoaof.html

C#:   File.Delete("a.txt");
来源：http://hz.daria6918.cn/gtkpqphmbi.html

[F07] 创建目录（含多级）
来源：http://hz.zhiwuduotai.top/gtptzcmcrn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258888.top/gtkafkvgen.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtgoquoytw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtvklpcsyv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtpldqknak.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtvxkylznt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtbbeynvvn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtbuizylmf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtigurbidc.html

[F08] 遍历目录
来源：http://hz.iojbl.cn/gtqpqvvtfo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtfququyqo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jyoumei.cn/gtbbkpkmyg.html

JS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtkyxnfbhu.html

TS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtdougxins.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtrxyoqdjx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtkjeuykos.html

Ruby: Dir.children("dir")
来源：http://hz.hnxiangtu.top/gthylnuhbg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtogxaazpt.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtwklkemiw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.snrcjt.cn/gtnktiafbi.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtriepemqb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gticzvupek.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtaritsven.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtxuabjzui.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yvedp.cn/gtwplbnkvp.html

Ruby: File.size("a.txt")
来源：http://hz.dianchejie.cn/gtlqtiocjs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daxiang520.top/gtigbdxnqd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtbbhaexod.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtminzgpca.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuxming.cn/gtcqdrfhkl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtkowyndki.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtpormrthy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guannengcc.top/gtdwyhmvat.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guowangkeji.top/gtbkivlbep.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtkpsilwzf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hfpthk.cn/gtzvigxjyy.html

[F11] 复制与移动文件
来源：http://hz.zhaomingkeji.xyz/gtzunfaceu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtinyzyhhv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtvixyxtfw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtxxutkonh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtlmjlevai.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtpvhhwseh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtyocvwjzv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtssncgpzz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtemuwgacr.html

[F12] CSV 读写
来源：http://hz.gzhubu.top/gtmrrxxfxe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yangfankeji.com/gtkefmakds.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtohvmhjmu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtthalbcht.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtjvoooxcd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtoqnrgvho.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtvlsziojc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gtbweqpjic.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtauiztunq.html

================================================================================
来源：http://hz.smart0.xyz/gtkuyindeq.html

G. 面向对象
来源：http://hz.jinqigfzy.top/gtbnnaiemk.html

================================================================================
来源：http://hz.hnqzz.top/gtgjibovvg.html

[G01] 定义类
来源：http://hz.havefunace.top/gtdanjnqqe.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtgcaexqrz.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtfmtnskyv.html

JS:   class User {}
来源：http://hz.wangshuangyany.cn/gtkagreykg.html

TS:   class User { name: string = ""; }
来源：http://hz.sysykeji.top/gtzexazavl.html


<!-- 参考信息 -->