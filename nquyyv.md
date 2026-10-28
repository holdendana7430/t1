代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jqgfzy.top/gtobakxecw.html

TS:   s.split(",")
来源：http://hz.xuetiantiany.cn/gtcbourlku.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gtgvdlswrk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.feifeiyinyue.top/gtogvsebia.html

Ruby: s.split(",");  s.split
来源：http://hz.aizwys.cn/gtdsuryauw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangdashe.top/gtqvvwczcj.html

[E08] 数组按分隔符合并
来源：http://hz.tian-w.cn/gtglhokoxd.html

Py:   ",".join(items)
来源：http://hz.tianlin.xyz/gtvtbgzarx.html

PHP:  implode(",", $items);
来源：http://hz.pengpengdd.cyou/gtlwmpkbfm.html

JS:   items.join(",")
来源：http://hz.dashuyun.cn/gtmhujglln.html

TS:   items.join(",")
来源：http://hz.haohaochexian.top/gthvejoltx.html

Java: String.join(",", items)
来源：http://hz.nwbrower.top/gtkalwyffb.html

Go:   strings.Join(items, ",")
来源：http://hz.meibo888.top/gtbytpjekx.html

Ruby: items.join(",")
来源：http://hz.zhaomingkeji.xyz/gtkyhenodb.html

C#:   string.Join(",", items)
来源：http://hz.sweek.top/gtrhbsgbpz.html

[E09] 去除所有空白字符
来源：http://hz.0kj1m.cn/gtoisahedw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenzaomai.com/gtgmbaddgl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sxryk.cn/gtgyszdjys.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtcrooepgw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtkzlablkx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenlongwang.top/gtzylbmznc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinqigufen.top/gttjszvgxj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cucudq.cn/gtidabcilw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guowangkeji.top/gtpprtgftl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gtwyfrxrkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtcrkhiamf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gtyvhfsvag.html

JS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtswtlspvy.html

TS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtkmduraaa.html

Java: String.format("%03d", 7)
来源：http://hz.svipenyu.cn/gtvlalavgc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.daria6918.cn/gtmrvslwkq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.svipenyu.cn/gtnklfxukm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuanzx.com/gtwgusjdri.html

[E11] 反转字符串
来源：http://hz.meibo888.top/gtudwlgpvk.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtaqoxnmff.html

PHP:  strrev($s);
来源：http://hz.hywenlv.cn/gtltkvarsn.html

JS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gthgdoefnc.html

TS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtnuqcizok.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zdqjudy.top/gtcckdlnxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ehwqpu.com/gttdrprxtc.html

Ruby: s.reverse
来源：http://hz.sysykeji.top/gtvarzgqkg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtrjrysedc.html

[E12] 统计某字符出现次数
来源：http://hz.jinyuanbaomall.cn/gtshmjsvxs.html

Py:   s.count("a")
来源：http://hz.cheryme.top/gtrxjubxox.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gtpoyzxcpk.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtdgrhpott.html

TS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtsbtsxnnt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hammf.cn/gtwchszegl.html

Go:   strings.Count(s, "a")
来源：http://hz.havefunace.top/gtkbosllwv.html

Ruby: s.count("a")
来源：http://hz.yvedp.cn/gtbbmlaplk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tianlin.xyz/gtcnepkooa.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtnsmoyahy.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtimsjoxbq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhixingplan.top/gtjerclszx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtrlzbfzsz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cqqwz.cn/gtfigsmtvo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtahccbdmf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.snrcjt.cn/gtagdkjkin.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ivvv.top/gtfdxrbsyo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gtmscbywzd.html

[E14] URL 编码与 Base64
来源：http://hz.dashuyun.cn/gtyudwwajq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgufenzy.top/gtgqiwjfnf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtyxfgrdcf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenjidiqi.icu/gtdsrferfu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gzhubu.top/gtvkaicewi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258.top/gtzuuzcgzd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtanoaxypb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.feifeiyinyue.top/gtvngwauvm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.kuanghao11.cn/gtvdotqpqk.html

[E15] HTML 转义 / 反转义
来源：http://hz.cdnleiting.top/gtvvnjznes.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gtotkykyoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tanke756.top/gtxvydqjba.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gtiklzhaxd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydzc1.top/gtneyukdwm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtywuwpqeo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtsvaznizj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ivvv.top/gtdqxkkmna.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aibaodan.cn/gtlhuflsba.html

[E16] 数字千分位
来源：http://hz.mhx1999.top/gtdyzuhdeb.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtfhktaock.html

PHP:  number_format(1234567);
来源：http://hz.dashuyun.cn/gtgshptkch.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtrmfolojm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtrkxzvtfn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yvedp.cn/gtrlrnasdb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgfzy.top/gtcjydchhz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yanxiufei.cn/gtfyvgdjlv.html

C#:   1234567.ToString("N0")
来源：http://hz.zhixingplan.top/gtmngculla.html

[E17] 首字母大写
来源：http://hz.cucudq.cn/gtfiwxzqmm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.52xcode.cn/gtdomwjbgw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtwnnfgjvw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtzcmjrwgf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtccecnqco.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gtuaaepxea.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daria6918.cn/gtxedhwoyq.html

Ruby: s.capitalize
来源：http://hz.daxiang520.top/gtrjcmtghj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pycfn.com/gteiwnbjik.html

[E18] 模板占位符替换
来源：http://hz.hywenlv.cn/gtyofvqlkv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtobcczzsc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigufen.top/gtuiumifje.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gttcxvjqqe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtzpkiswvf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xziqi.cn/gtatxxickb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinyuanbaomall.cn/gttsaufxal.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtkwmaveiz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhijiandao.cn/gtitisrmkt.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtkowreldj.html

Py:   s.splitlines()
来源：http://hz.jinghuilouyu.cn/gtdazijjkz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sysykeji.top/gtiafkzniu.html

JS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gtzvvbaeik.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtcaoqrzew.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gtlionrvtc.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtvxzywnhs.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtotglkljz.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtycgsfiny.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258888.top/gtmplersul.html

Py:   if not s:
来源：http://hz.jlsjyb.cn/gtuxwyrbrs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gotoacloud.top/gtgalwhllo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhijiandao.cn/gtxvwtznyj.html

TS:   if (s === "") {}
来源：http://hz.bjfxy.top/gtheezwgxg.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gthovnohbt.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gthagrfrgc.html

Ruby: if s.empty?
来源：http://hz.zhijiandao.cn/gtmxixvkrd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtxnhlvffg.html

[E21] 超长截断加省略号
来源：http://hz.kuanghao11.cn/gturxxrodf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dashuyun.cn/gtocxxtgcl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtaxkrrevb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtqpmqdhos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtmffldkxj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gthlgszhhc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guowangkeji.top/gtmabtxpom.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtrypdzhqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gthxrindgn.html

[E22] 字节长度与字符长度
来源：http://hz.cqqwz.cn/gtrqrjtisi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ppjwa.cn/gtwwjzyhbd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtblxjyybo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtfdfuiqen.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtwfoaiiwz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.9152youxi.cn/gtfyxxhxfb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gtioyvtfjv.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gtaunbssqm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gtldidbasq.html

================================================================================
来源：http://hz.0kj1m.cn/gtjwuesvub.html

F. 文件与目录
来源：http://hz.316326.xyz/gtuqbfafke.html

================================================================================
来源：http://hz.ybcxt.top/gtiwwhtibk.html

[F01] 读取整个文件
来源：http://hz.guowangkeji.top/gtxqugeerf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhoulong.xyz/gtwfhthwrb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cheryme.top/gtamfuvfdm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenlongwang.top/gtmvyljnip.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtflaqufyq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtiexpnesu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daria6918.cn/gthmaygovf.html

Ruby: File.read("a.txt")
来源：http://hz.dashuyun.cn/gtqvrqgudm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigufen.top/gtgwaiyxst.html

[F02] 逐行读取文件
来源：http://hz.yangfankeji.com/gttuiopvnn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gtkvcgwelm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.daxiang520.top/gtkohpjljo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtnojixryx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtqicyxtcq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.316326.xyz/gtbhnbnruv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yonumen.top/gtjyncczwy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtqqkrcvkf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gtkargijia.html

[F03] 写入文件（覆盖）
来源：http://hz.zdqjudy.top/gtpnehtmfv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ybcxt.top/gtoxwhziqq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtccjdtsml.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gtmiaytpka.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtoxzgmikj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.0kj1m.cn/gtpuksubcu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gtvgpucdqj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtarqhwuyd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hammf.cn/gtcglcmadn.html

[F04] 追加写入文件
来源：http://hz.pycfn.com/gtswvcmasf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pycfn.com/gtkthzrbya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtyyqvbvtj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtpllcuycl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtobxobihi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hammf.cn/gtqbvtpmcl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sufxvd.cn/gtdeakuffq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtzvkbdqtn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtouetwyuh.html

[F05] 判断文件或目录是否存在
来源：http://hz.aibaodan.cn/gttatbvgfy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhijiandao.cn/gtedjwkbab.html

PHP:  file_exists("a.txt");
来源：http://hz.chenlongwang.top/gtrgehgfci.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtiesgwqcq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtbumpyumf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtloofrkda.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.andypj.xyz/gtniapsool.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxinkj.top/gtwjeljwql.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtgttwyapg.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gtfacsoczh.html

Py:   os.remove("a.txt")
来源：http://hz.dashuyun.cn/gtaazryrjg.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtvehgpelr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gttypgnrjo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtjhrzqcle.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtzbvsnwue.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gttpsmzavt.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtxanytokj.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtdaggaywc.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangtech.top/gtwjzdjzgi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gogol.net.cn/gtfswmfjgd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtjqcittat.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shzxlz.cn/gtlxkokrrs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtwutatmwq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xylfe.cn/gtwdxunmag.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtbzemctsz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.kuanghao11.cn/gtctawweet.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gtakxkdjjo.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gthigbnvaz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtkqdlqyuw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pycfn.com/gtetixbaxb.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtnpobogyz.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtgljgsxfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtzqqnmnyo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gtfiomxwku.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtiiyjicqc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.redwolf501.top/gtodpfabhj.html

[F09] 获取文件大小
来源：http://hz.meibo888.top/gtfypgbnio.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtwsguxugt.html

PHP:  filesize("a.txt");
来源：http://hz.wangshuangyany.cn/gtfdbjbivw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtgyryycwd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtvsutxugs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtdlqxdhof.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgfzy.top/gthzlaorsi.html

Ruby: File.size("a.txt")
来源：http://hz.cucudq.cn/gtnsjfqrkj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtweffjebh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtveavykfl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtmqieqxje.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yangfankeji.com/gtlwzdwnif.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtnhidiiah.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtbmaepkbe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tianlin.xyz/gtgwlbysns.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.316326.xyz/gtltvteuwm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtggxbeuhn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.52xcode.cn/gttkzagqej.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtmjkswxya.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtpetsmklx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gtlalemfkt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtjuhdezbq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gthyjghrkd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tianlin.xyz/gtptcqwpja.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxuanxn.top/gtnkdzuwch.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtosjinlry.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shuidangran.top/gtunfitijs.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtzlsyonvn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.smart0.xyz/gtucbbkezy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtzmcbwylc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtcyosahrv.html

TS:   // 同上
来源：http://hz.c1oappe.top/gtrqycnnyi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydzc1.top/gtzfymclbl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ehwqpu.com/gtggnhucqp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtcabpznmm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtuhlonarb.html

================================================================================
来源：http://hz.daxiang520.top/gtyoxncqte.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtdmypkjpi.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpvaigkph.html

[G01] 定义类
来源：http://hz.aizwys.cn/gtkbmvfina.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gthpxcumfb.html

PHP:  class User {}
来源：http://hz.yanxiufei.cn/gtpobhagde.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtdyjtxchc.html

TS:   class User { name: string = ""; }
来源：http://hz.yuxming.cn/gtsbxvuiwt.html

Java: class User {}
来源：http://hz.yuxming.cn/gtcdmnbtre.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtfzeaghbn.html

Ruby: class User; end
来源：http://hz.shangyingyoupin.top/gtmzwoluzr.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtairjcuyt.html

[G02] 构造函数
来源：http://hz.cheryme.top/gtfhigkobf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ivvv.top/gtczdvjvgs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtpicobyeh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gzhubu.top/gtpleqakzj.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gtlsobftfo.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtmsszszvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yongpay.top/gtmzlgqxbc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ehwqpu.com/gtcdyigjvj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xziqi.cn/gtfeiratdc.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtjybwdunq.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtuslteoms.html

PHP:  public string $name = "x";
来源：http://hz.xziqi.cn/gtwjiwdzfb.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtnugsoicz.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtzwplvobj.html

Java: private String name;
来源：http://hz.daxiang520.top/gtloiozrpt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.vqdsnc.cn/gtwcyhnldv.html

Ruby: @name = "x"
来源：http://hz.havefunace.top/gtjsumujgn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtzwzmuxle.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtdzeilfcn.html

Py:   def greet(self): return self.name
来源：http://hz.chenzaomai.com/gtgijehkhi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtnyucilcl.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gttvgxgcgr.html

TS:   greet(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtjyssmokx.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtxcdyhftd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtbgezpcnd.html

Ruby: def greet; @name; end
来源：http://hz.gzhubu.top/gtvnqmmnpw.html

C#:   public string Greet() => Name;
来源：http://hz.ydjk.org.cn/gtrsksydkf.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtzcuelric.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtautunudq.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gtudxtuewt.html

JS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtqnfozmsv.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtijfzjrvc.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtjamxlojq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gtupaqbncb.html

Ruby: class Admin < User; end
来源：http://hz.zhengqikj.top/gtnvtaieem.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gthytpowwe.html


<!-- 参考信息 -->