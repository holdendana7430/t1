代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtqeripspg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dashuyun.cn/gtedofvmwr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jianghu66.top/gtqqmhykmk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pycfn.com/gtgogvvcxb.html

[E06] 替换子串
来源：http://hz.jinyuanbaomall.cn/gtumgxvpqj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xziqi.cn/gtimriwkfi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gaohongyu789.top/gtmdqkxrwe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtapmpuylo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtnqdowejy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gthmkqphuk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenzaomai.com/gttwfspftq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.andypj.xyz/gterulyvty.html

C#:   s.Replace("a", "b")
来源：http://hz.yanxiufei.cn/gtogkimdpn.html

[E07] 按分隔符拆分
来源：http://hz.gogol.net.cn/gtejcynidp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258888.top/gtjbfvjaaq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.redwolf501.top/gtudjacxah.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hammf.cn/gtgqwxknxd.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtembdligm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.meibo888.top/gtsgztbpac.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ehwqpu.com/gttefarlgk.html

Ruby: s.split(",");  s.split
来源：http://hz.tian-w.cn/gtrcbosdhb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zdqjudy.top/gtjerypfhf.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gtxpycggwc.html

Py:   ",".join(items)
来源：http://hz.andypj.xyz/gtfuzhvxmh.html

PHP:  implode(",", $items);
来源：http://hz.ydzc1.top/gtlwmblluc.html

JS:   items.join(",")
来源：http://hz.haohaochexian.top/gtyzdiaipd.html

TS:   items.join(",")
来源：http://hz.redwolf501.top/gtoeegudwn.html

Java: String.join(",", items)
来源：http://hz.jqgufenzy.top/gtcisgghnd.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangtech.top/gtwldkyagy.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtzizrmmjo.html

C#:   string.Join(",", items)
来源：http://hz.nanxinkj.top/gtkiuzqtej.html

[E09] 去除所有空白字符
来源：http://hz.wangshuangyany.cn/gtzwixhipg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtuxorcrfg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.haohaochexian.top/gtdylpfuym.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.0kj1m.cn/gtbdsouvzd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtvemmldir.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aibaodan.cn/gtuqtcanem.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.feifeiyinyue.top/gtcgoaqbmi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gteburwhpv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangtech.top/gtcswxalak.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtteinlvrs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtwnyasziv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gtgprpmpps.html

JS:   "7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtgiohkmye.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtctadznbp.html

Java: String.format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtyugonowz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtknrnywlt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yvedp.cn/gtdwnjsewn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dianchejie.cn/gtfqvixeur.html

[E11] 反转字符串
来源：http://hz.hysaishi.cn/gtussdcekd.html

Py:   s[::-1]
来源：http://hz.ehwqpu.com/gtopmbpjfy.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtwtsnzrkp.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtweyiktum.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtbwksulxw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sweek.top/gtyewzbzic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.fengsongda.top/gtiksjxzop.html

Ruby: s.reverse
来源：http://hz.xinyue.icu/gtqajmjvgl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtyxrzwnpf.html

[E12] 统计某字符出现次数
来源：http://hz.jlsjyb.cn/gtmyliatjo.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtgssquhuy.html

PHP:  substr_count($s, "a");
来源：http://hz.cdnleiting.top/gtxzzwosuc.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtyxnoykwj.html

TS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtfqtgtnwc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangdashe.top/gtcpqabafm.html

Go:   strings.Count(s, "a")
来源：http://hz.cucudq.cn/gtuonczbbc.html

Ruby: s.count("a")
来源：http://hz.ydjk.org.cn/gtfbrrwngq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sufxvd.cn/gtgytygdgt.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtmfnaynnq.html

Py:   for ch in s: print(ch)
来源：http://hz.ydzc1.top/gtcvyiuosu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtsplndzdk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gthqbqyylj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtuiobhtlq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxuanxn.top/gtmtlolahw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtfwsqddiw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gttfmttzci.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtmbqzhwhc.html

[E14] URL 编码与 Base64
来源：http://hz.chenlongwang.top/gttsfhwywu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtxxmhjcyo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangdashe.top/gtlmkdipkr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.smart0.xyz/gtrcsnkmpx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yanxiufei.cn/gtuqmlblcp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gttowiypkr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yangfankeji.com/gthztgnlir.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtgfmedcxx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtkehzuyse.html

[E15] HTML 转义 / 反转义
来源：http://hz.xinyue.icu/gtdrnxrirv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtdaovmygs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zdqjudy.top/gtnnsbstmz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nanxuanxn.top/gtsdwtglxm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtsrjscetp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tian-w.cn/gtqenawhok.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtsaeksyri.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.iojbl.cn/gtwnkpzkmt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtpvmmaoyz.html

[E16] 数字千分位
来源：http://hz.jinqigfzy.top/gtlzhenxdn.html

Py:   f"{1234567:,}"
来源：http://hz.wangshuangyany.cn/gtubilrdev.html

PHP:  number_format(1234567);
来源：http://hz.sweek.top/gtzocajhpy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtviinvrdi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtcqtgwevf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.andypj.xyz/gtalysbvta.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtmehrqsqt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zdqjudy.top/gtptssrehj.html

C#:   1234567.ToString("N0")
来源：http://hz.yanxiufei.cn/gttyaraobf.html

[E17] 首字母大写
来源：http://hz.yongpay.top/gtjdryqtcf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jlsjyb.cn/gtwxwrqkgj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jiagoushi.top/gtrcuiocjg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtbzyptuku.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtfindbchc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtlmintrep.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtvsgbxsck.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gthbfnwakp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtlbzgjayg.html

[E18] 模板占位符替换
来源：http://hz.yuanzhike.top/gtuhwmddfv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.havefunace.top/gtdkniruzn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtkvqpjbea.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtprzspwhe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtteceoduu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtszombcqg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cqqwz.cn/gtdecfipje.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shzxlz.cn/gtkuamqyuu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.svipenyu.cn/gtieiesywn.html

[E19] 多行文本按行拆分
来源：http://hz.cdnleiting.top/gtxpbgqtcn.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gtimtigazc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nwbrower.top/gtacnbslzf.html

JS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtogbjlyjm.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtudomhres.html

Java: s.lines().toList()
来源：http://hz.xylfe.cn/gtykwvziie.html

Go:   strings.Split(s, "\n")
来源：http://hz.cheryme.top/gtkrfuzlwx.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtsgchcqgx.html

C#:   s.Split('\n')
来源：http://hz.shangyingyoupin.top/gtwouczwjh.html

[E20] 判断字符串是否为空
来源：http://hz.quarkkingdee.top/gtxtfmnjag.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtgnphiwcq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtlworxqbm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gogol.net.cn/gtmoxtafls.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtnvfgxnxw.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtxiqvkxei.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtktnmccub.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtzmnqgfoi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.c1oappe.top/gttucbfswf.html

[E21] 超长截断加省略号
来源：http://hz.mhx1999.top/gttrthtcbq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tianlin.xyz/gtfuomsmzk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gzhubu.top/gteelgriha.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtuibarhku.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gttoomsgxr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtsorjeyfn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gtuzsddiwr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gtotkfksjq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtwqnmnfai.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtcofuniez.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtiavlgamm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtwkzbskur.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtsggljzuh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtnjkulbos.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nwbrower.top/gtcutegarj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fzhhl.top/gtuvgmlcga.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuanzx.com/gtsfgtxsex.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtvdhnzuka.html

================================================================================
来源：http://hz.meibo888.top/gtqwwvdyya.html

F. 文件与目录
来源：http://hz.cashguo.top/gtiejosdjj.html

================================================================================
来源：http://hz.nanxinkj.top/gtityqwdbl.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtslrfdify.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dianchejie.cn/gtvbputfqh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gttyjjnnkp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangtech.top/gttizolqhw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigufen.top/gtycbxfncz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtwbsjjcxw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtlkzlsrwp.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gttczkabos.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ehwqpu.com/gtscmafocj.html

[F02] 逐行读取文件
来源：http://hz.yanxiufei.cn/gtqkusrnsl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gtujxnaxpt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sxryk.cn/gtcylpqkbo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtpmhbbjqy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtbzjxkysw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtoaxuvggz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtyrjacnqh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hammf.cn/gtibnzroju.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuxming.cn/gtcjrpdsmt.html

[F03] 写入文件（覆盖）
来源：http://hz.redwolf501.top/gtrftojwwf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinyuanbaomall.cn/gtdapwaqbl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtdxzlwxhb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gttakpbvat.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtdvevcmkx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenlongwang.top/gtyddcozug.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtlruvnahj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigufen.top/gtwpphzneh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtlrucodwo.html

[F04] 追加写入文件
来源：http://hz.yonumen.top/gtszibyfrp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gotoacloud.top/gtxraocrlp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yvedp.cn/gtkyfawohw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtkgonxbrx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtvnlcpmwx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydjk.org.cn/gtsggeppuf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtbwkprqee.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yvedp.cn/gtulilwdto.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.bjfxy.top/gtzwavrtpv.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxinkj.top/gtfrkvxdqk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gtcbozxhzp.html

PHP:  file_exists("a.txt");
来源：http://hz.shangyingyoupin.top/gttyhxmqqz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtmyxblheh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtnmzjuvjj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtixsxlgcp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtxylyexbc.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtgbsgbnwo.html

C#:   File.Exists("a.txt")
来源：http://hz.daxiang520.top/gtblwspzss.html

[F06] 删除文件
来源：http://hz.iojbl.cn/gtvsjfchfl.html

Py:   os.remove("a.txt")
来源：http://hz.hnxiangtu.top/gtsvnhvmyc.html

PHP:  unlink("a.txt");
来源：http://hz.cqqwz.cn/gtlgowukao.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtjfssroes.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtrmunkwpv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtjquaadfl.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtlakhgkpd.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gtfunzbnxa.html

C#:   File.Delete("a.txt");
来源：http://hz.cashguo.top/gtlqgmzvsi.html

[F07] 创建目录（含多级）
来源：http://hz.hywenlv.cn/gtoltvmzha.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dianchejie.cn/gtefusynaf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daxiang520.top/gtzcyyugat.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtgatdhpdr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtbnziuzlk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuetiantiany.cn/gttnxwqzae.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shanyushiyangkeji.top/gtoreyubnl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guannengcc.top/gtgvbygfhz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangtech.top/gtkoqczmwl.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtuslswshi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ybcxt.top/gtfoktwaib.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fengsongda.top/gtmtucqaet.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtuqugmvti.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtyfphuydj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtzaksmywf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ehwqpu.com/gtbxkxprbe.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtyteevngp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gthmoriaun.html

[F09] 获取文件大小
来源：http://hz.meibo888.top/gtmunzoike.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gttpwxktzd.html

PHP:  filesize("a.txt");
来源：http://hz.daxiang520.top/gtreyaiegl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtvfqtctfb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtfqqkovnq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtotgwegju.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gthegurovm.html

Ruby: File.size("a.txt")
来源：http://hz.sysykeji.top/gtfyxanbyk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtoclmjrgz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gtlwxkycvr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtcsvtzhnc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.feifeiyinyue.top/gtmusdkwtv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtnshdpmde.html

TS:   path.extname("a.txt")
来源：http://hz.smart0.xyz/gticktzapv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtdrapczvx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gogol.net.cn/gtgxfioedf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtsjaobbil.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.9152youxi.cn/gtfdvmkcvy.html

[F11] 复制与移动文件
来源：http://hz.jianghu66.top/gtdammmeyp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtzpwuduei.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangtech.top/gtqtukqsat.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtwujhmymd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtakcjqdvs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtsqsizlmw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtlmfldyem.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtzrqjkatt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gtqpbbmjvm.html

[F12] CSV 读写
来源：http://hz.hysaishi.cn/gtapxgvvpm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yanxiufei.cn/gttatnzcmg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cqqwz.cn/gtacilmgpa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtdjfyrtfv.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtgtpvmzxm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.daxiang520.top/gtncirypyq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtojecemzi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fengsongda.top/gtfpcgowzy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shzxlz.cn/gtxypqctlm.html

================================================================================
来源：http://hz.yueranfly.top/gtuklmhjqs.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtlzuuwuea.html

================================================================================
来源：http://hz.fzhhl.top/gtjpwowtml.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtkjundyqz.html

Py:   class User: pass
来源：http://hz.zhongyouzk.top/gtztqeiqfy.html

PHP:  class User {}
来源：http://hz.cucudq.cn/gtyvpkaocp.html

JS:   class User {}
来源：http://hz.ybcxt.top/gtolvjsxmx.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtiiibxdqg.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtumdlprvz.html

Go:   type User struct { Name string }
来源：http://hz.chenjidiqi.icu/gtconsjxdt.html

Ruby: class User; end
来源：http://hz.jinqigufen.top/gtiebctvar.html

C#:   class User {}
来源：http://hz.jinghuilouyu.cn/gtbdvkopwi.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtypczxmmr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cashguo.top/gtrbxyrjob.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtqrsxapea.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gthvtlhyyl.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gteplrrqnz.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtbeeqhaxj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ehwqpu.com/gtowhydmov.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtwylkzgmv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtdfzkbrdl.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtlwgmscfs.html

Py:   self.name = "x"
来源：http://hz.hongshengwenyu.top/gtikzouhtz.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtzhbqrups.html

JS:   this.name = "x";
来源：http://hz.meibo888.top/gtehtnijes.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtscghzxbb.html

Java: private String name;
来源：http://hz.jianghu66.top/gtzkixcjbv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sweek.top/gttyhgdznn.html

Ruby: @name = "x"
来源：http://hz.jinghuilouyu.cn/gtwoydkamh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtgelfmdoz.html

[G04] 定义方法
来源：http://hz.yuanzhike.top/gtngoefnde.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtxxkekbla.html


<!-- 参考信息 -->