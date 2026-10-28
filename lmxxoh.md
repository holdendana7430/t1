代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtkpfmmvmb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sweek.top/gtbgvpgghx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gotoacloud.top/gtewdfwvcc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.kuanghao11.cn/gtwrvtfhud.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtwzmookap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yvedp.cn/gtiswiyced.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenjidiqi.icu/gtwasczibi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtzybjacvm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gthymskfpx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtwcqpoqqx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gthlfubqox.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ehwqpu.com/gtgptqynxq.html

C#:   s.Replace("a", "b")
来源：http://hz.ydjk.org.cn/gtmzgncjfx.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gtcsfvorfj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gaohongyu789.top/gtfrfsxugu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cqqwz.cn/gtkdjpxajo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gaohongyu789.top/gtpdrasdya.html

TS:   s.split(",")
来源：http://hz.feifeiyinyue.top/gtlusgqqui.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hammf.cn/gtjbcsrppp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.andypj.xyz/gtxafuhvzz.html

Ruby: s.split(",");  s.split
来源：http://hz.guannengcc.top/gtsfbndeld.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daria6918.cn/gtgyojkznk.html

[E08] 数组按分隔符合并
来源：http://hz.hammf.cn/gtniutkkeq.html

Py:   ",".join(items)
来源：http://hz.52xcode.cn/gtldxukofp.html

PHP:  implode(",", $items);
来源：http://hz.quarkkingdee.top/gtxmkskmmi.html

JS:   items.join(",")
来源：http://hz.aibaodan.cn/gtulpserxd.html

TS:   items.join(",")
来源：http://hz.iojbl.cn/gtnioaluou.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtemozwbtf.html

Go:   strings.Join(items, ",")
来源：http://hz.ehwqpu.com/gtkuzlvycv.html

Ruby: items.join(",")
来源：http://hz.nwbrower.top/gtdwpvzdif.html

C#:   string.Join(",", items)
来源：http://hz.yuxming.cn/gtkjtizrlq.html

[E09] 去除所有空白字符
来源：http://hz.hammf.cn/gtuewmfgnr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tian-w.cn/gtcafthhro.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gthyjmzyjo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gteeyorsda.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtvhffxzmj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuetiantiany.cn/gtbcuykxap.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ivvv.top/gtsxyjduut.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sufxvd.cn/gtcufbrbrc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fzhhl.top/gtdtwcrbtz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtyjtydfxu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sweek.top/gtcgmclutn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnqzz.top/gtxjmlarnw.html

JS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtnnyqvtpa.html

TS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gttndkxfbk.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtehhgpvcn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.snrcjt.cn/gtmptehzye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gtcskdzpyr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tian-w.cn/gtuftjhuxy.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtffhhcwbv.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtchngameq.html

PHP:  strrev($s);
来源：http://hz.wangshuangyany.cn/gteciorxgr.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gttzxbkkgd.html

TS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtjawcprjk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhaomingkeji.xyz/gtxbsfneow.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangshuangyany.cn/gtvhgssbgu.html

Ruby: s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtqaycvvra.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gtmspwizku.html

[E12] 统计某字符出现次数
来源：http://hz.yueranfly.top/gttvluqawa.html

Py:   s.count("a")
来源：http://hz.cucudq.cn/gtcwycnvlz.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gtjfknwptw.html

JS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gticvltwah.html

TS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtvvhucwyx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.svipenyu.cn/gtabuhonbw.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gtavekvqdb.html

Ruby: s.count("a")
来源：http://hz.zhengqikj.top/gtplocemoj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gtnmsuwksq.html

[E13] 逐字符遍历
来源：http://hz.zycfv.cn/gtpmooobhq.html

Py:   for ch in s: print(ch)
来源：http://hz.cucudq.cn/gtjybxbapl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yangfankeji.com/gtlsvwsgci.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtjhnplqry.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtoedptaqf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shuidangran.top/gtgmgblgfu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuanzx.com/gtlxeiadpz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhijiandao.cn/gtrhxisigh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hfpthk.cn/gtmokncswg.html

[E14] URL 编码与 Base64
来源：http://hz.gogol.net.cn/gtdhzdgcji.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yangfankeji.com/gtqrjffevt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aizwys.cn/gteazropzf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.quarkkingdee.top/gtfomvmupv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtqynveodd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ehwqpu.com/gtwgtejcuv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenlongwang.top/gtjwrvlkdq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuanzhike.top/gtepcnemfp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gzhubu.top/gthchodyzg.html

[E15] HTML 转义 / 反转义
来源：http://hz.zdqjudy.top/gtopygrwqm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yangfankeji.com/gtdvzaelbq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuxming.cn/gttuwmrxyn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cheryme.top/gtqxmiberu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gttzlxblaj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gteifnzblm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gtadtmrfrp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fzhhl.top/gtqovmbnzl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhongyouzk.top/gtertqmsji.html

[E16] 数字千分位
来源：http://hz.havefunace.top/gtkzucdijr.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtlifipgxd.html

PHP:  number_format(1234567);
来源：http://hz.zhijiandao.cn/gtsooyuwmc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtwigtoxta.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtawzjjonk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cdnleiting.top/gtynonrkcs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhongyouzk.top/gtkjzybhcj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtshpqfdsv.html

C#:   1234567.ToString("N0")
来源：http://hz.cucudq.cn/gtwkfyfqtu.html

[E17] 首字母大写
来源：http://hz.hongshengwenyu.top/gtfmthznqd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gtgtmwgcja.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtwpstmdon.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gtgumvticm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtdgnzsggq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuanzhike.top/gtmaymgfus.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtvtbidtnx.html

Ruby: s.capitalize
来源：http://hz.ehwqpu.com/gtqoglfuwv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxuanxn.top/gtqolsxudc.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gtvuzknbjn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.316326.xyz/gtjuhrxmdv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtmsxjeeoy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gterkrmabh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sxryk.cn/gtqdrnafsy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guannengcc.top/gtousghstv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtutryhmqv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ivvv.top/gtgzcovpec.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.andypj.xyz/gtltjoqpqp.html

[E19] 多行文本按行拆分
来源：http://hz.9152youxi.cn/gtctjqzzuu.html

Py:   s.splitlines()
来源：http://hz.svipenyu.cn/gtiftlmayl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hammf.cn/gtqernlxgq.html

JS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtxpcoygoe.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhaomingkeji.xyz/gtlbjauvwg.html

Java: s.lines().toList()
来源：http://hz.cucudq.cn/gttpsbsfgh.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtgirxoale.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gthiegaryd.html

C#:   s.Split('\n')
来源：http://hz.xylfe.cn/gtcznrxffa.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gtxiouemtq.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtshekvila.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cucudq.cn/gttgvyevkk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ppjwa.cn/gtgryigtgh.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtulebgxjn.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtbieitflr.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtwvagvkuc.html

Ruby: if s.empty?
来源：http://hz.gogol.net.cn/gtnuddmwjj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sufxvd.cn/gtjfnaszuv.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtrrrqhtbp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zycfv.cn/gtimuntvbk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hysaishi.cn/gtdffgvaov.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtpxldzhhz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtfnvsksxr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtymxzrqfh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gtwkhafllh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gtkoaykxrt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtolrpdmhv.html

[E22] 字节长度与字符长度
来源：http://hz.pengpengdd.cyou/gtuqulmnut.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhijiandao.cn/gtgqvrzgws.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtmgceywni.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtojkwiauv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtznqptnav.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtxxyappew.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xingfuxueyuan.xyz/gtyeojdgat.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenlongwang.top/gtsyfjdouz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.kuanghao11.cn/gtbkfrxmnx.html

================================================================================
来源：http://hz.quarkkingdee.top/gtuszqbrtt.html

F. 文件与目录
来源：http://hz.wangdashe.top/gtsqixzmbl.html

================================================================================
来源：http://hz.cheryme.top/gtminzpmgs.html

[F01] 读取整个文件
来源：http://hz.zhongyouzk.top/gtumxgtfjk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dashuyun.cn/gthpygfqig.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtuwzxpnyd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ppjwa.cn/gtlzouklwu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tianlin.xyz/gtftttvztz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtrctatrzx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtpelgmejb.html

Ruby: File.read("a.txt")
来源：http://hz.hywenlv.cn/gtjouhqdtp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ybcxt.top/gtpsapjqhm.html

[F02] 逐行读取文件
来源：http://hz.mhx1999.top/gtemsbzqar.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nwbrower.top/gtgnegwxxr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yangfankeji.com/gtdmqhrdvq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtfvsezroj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtatlecypd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtbjclzmch.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gtvssfhvgf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zycfv.cn/gtvimbfjwm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtqznufnom.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gtqlgupdhf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenzaomai.com/gtztcqrvpy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtqpubcpjx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtzkmjxldo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtwnxgwypf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fzhhl.top/gtyfsfuwcj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jlsjyb.cn/gtyrbdwmop.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yvedp.cn/gtnfbxagiw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhixingplan.top/gtkmmoymhj.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtqzggkhod.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtoasavaam.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtmfzgtcqr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yanxiufei.cn/gtfmnqqqsw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtwiesbaor.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhengqikj.top/gtjmgjogjg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtmnmhmbso.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtqezcltmq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.smart0.xyz/gtwycgpjhy.html

[F05] 判断文件或目录是否存在
来源：http://hz.daria6918.cn/gtpwyfsvqm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.kuanghao11.cn/gtjcznmwdd.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtbhchnzzt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtvxwhieih.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtbxoekfwj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtfsykwbjn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.0kj1m.cn/gtyrexzmer.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinghuilouyu.cn/gtmkmavhmw.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtijutrhmm.html

[F06] 删除文件
来源：http://hz.xuanzx.com/gtuapbutlu.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtvwvmnyrv.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtiauiniti.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtljodnbdh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gthgrtgsce.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtetavfudg.html

Go:   os.Remove("a.txt")
来源：http://hz.jiagoushi.top/gtzgvbowcf.html

Ruby: File.delete("a.txt")
来源：http://hz.jianghu66.top/gtjvqmhyyh.html

C#:   File.Delete("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtllcvunsg.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtzidohtrv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gtmqmwfkrl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.vqdsnc.cn/gtamizvblv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtrdcudnld.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hywenlv.cn/gtoqiofiea.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.bjfxy.top/gttxrzernv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.haohaochexian.top/gtutduqpfg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuetiantiany.cn/gtrwuohxit.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yangfankeji.com/gttvytfwnz.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtnaonasmt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtcchqbqpj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jianghu66.top/gtubnwlokx.html

JS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtwakpqgby.html

TS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtpneaeimi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtmqjnldkh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ybcxt.top/gtbsdwjtzq.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gtmugbluil.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gtybaybjyg.html

[F09] 获取文件大小
来源：http://hz.tanke756.top/gtunoacity.html

Py:   os.path.getsize("a.txt")
来源：http://hz.iojbl.cn/gtowqvbziv.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtghbjuzek.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtcufzuwxy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtmeeratpc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gttbgzxsip.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtsdulagdg.html

Ruby: File.size("a.txt")
来源：http://hz.fengsongda.top/gtmklqeijo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gttdrnfaso.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtiuzxhrdw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtfqjoysue.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangkeji.top/gtvkoiynsa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtednuhgqu.html

TS:   path.extname("a.txt")
来源：http://hz.quarkkingdee.top/gtwvxbuohu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gttirkijkv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtuhdohhqk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtirureihc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtrnkdczqn.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtfngohiiz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtxwvsbzqo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jlsjyb.cn/gtrbiugeij.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtgiiwwveb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtstobjbqp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtibdlqvhq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhoulong.xyz/gtxgumxkpk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtzcuegowx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xziqi.cn/gtcrsfvgnj.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gtawwsdhmd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtxpbtpesu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hysaishi.cn/gtecaxurny.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hywenlv.cn/gtdatgrghk.html

TS:   // 同上
来源：http://hz.yj20258888.top/gtpxpbjxmc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yuanzhike.top/gtqcowpycj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtcilktemt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuanzhike.top/gtvbbgwuon.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtrnnjlsvy.html

================================================================================
来源：http://hz.yuxming.cn/gtsduvoxsc.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtmrgnyytg.html

================================================================================
来源：http://hz.yj202588.top/gtxveerpcz.html

[G01] 定义类
来源：http://hz.pengpengdd.cyou/gtikvtgmji.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtwchvkhxz.html

PHP:  class User {}
来源：http://hz.zhoulong.xyz/gtdhcgxmuh.html

JS:   class User {}
来源：http://hz.316326.xyz/gtqvalfyfj.html

TS:   class User { name: string = ""; }
来源：http://hz.ydjk.org.cn/gtrmhizfgq.html

Java: class User {}
来源：http://hz.ydzc1.top/gtycusfscg.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtzpncabjk.html

Ruby: class User; end
来源：http://hz.cheryme.top/gtdlcvitfp.html

C#:   class User {}
来源：http://hz.chenlongwang.top/gtftzrcpnl.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtprrpasso.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydjk.org.cn/gtnzrcmuvn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtedxvdtzw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtqecuxeuz.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gtpglbrazl.html

Java: User(String name) { this.name = name; }
来源：http://hz.yongpay.top/gtcfbptbss.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cqqwz.cn/gtnhyyrsnd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtdettsetk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtldydwibo.html

[G03] 实例属性
来源：http://hz.yj202588.top/gtsmupwodo.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gtnjzahscd.html

PHP:  public string $name = "x";
来源：http://hz.9152youxi.cn/gtpvnjerch.html

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gthfobfylv.html

TS:   name: string = "x";
来源：http://hz.wangshuangyany.cn/gtritpkirs.html

Java: private String name;
来源：http://hz.cucudq.cn/gtozheqprl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtirvnzbov.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtxujhhhgc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nwbrower.top/gttsgnfajy.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtmvgvzfrv.html

Py:   def greet(self): return self.name
来源：http://hz.hammf.cn/gtkhhtjket.html


<!-- 参考信息 -->