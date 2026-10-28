代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtyobcuztw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gtulmodrpa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtineuhizt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhiwuduotai.top/gttshmotst.html

[E06] 替换子串
来源：http://hz.tanke756.top/gtxlvobpvc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtfbvbyjos.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgfzy.top/gtxyyfnwsi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtfnibyooz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtgnyvwvyg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtyxuaayxz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtwzrdwaco.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gttsmhskwy.html

C#:   s.Replace("a", "b")
来源：http://hz.ydjk.org.cn/gtttbhuriq.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gtksujgswp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gtturahrrm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.daria6918.cn/gtjiqjdwxf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinyuanbaomall.cn/gtsckiuwmg.html

TS:   s.split(",")
来源：http://hz.ivvv.top/gtgyaacdtq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cheryme.top/gtrfxtjgfr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.0kj1m.cn/gtiaiitznz.html

Ruby: s.split(",");  s.split
来源：http://hz.haohaochexian.top/gteujhzecn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fengsongda.top/gtkzgmijwq.html

[E08] 数组按分隔符合并
来源：http://hz.cucudq.cn/gtsrqwimjt.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gtgghsleop.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtoyogvgvf.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtmhjfloce.html

TS:   items.join(",")
来源：http://hz.nanxuanxn.top/gtrmsdpvlw.html

Java: String.join(",", items)
来源：http://hz.shangyingyoupin.top/gtarhghfxe.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtdvbbppkg.html

Ruby: items.join(",")
来源：http://hz.fzhhl.top/gtrvfxadzw.html

C#:   string.Join(",", items)
来源：http://hz.zhongyouzk.top/gttiraaaqw.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gttnrlmebw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinqigfzy.top/gtjhoqyvce.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tanke756.top/gtovyzhzpt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtbfqermzj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtgjwrrfvo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.mhx1999.top/gtdfepdncr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtdpihwisb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tanke756.top/gtqgubitps.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cucudq.cn/gtdihujuvk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhengqikj.top/gtrgntyivz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jiagoushi.top/gtdgsbkwzb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hfpthk.cn/gttlznnvjt.html

JS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtrcrzxruv.html

TS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtnldeldas.html

Java: String.format("%03d", 7)
来源：http://hz.xylfe.cn/gtmbdvfida.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gthdqypumz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.meibo888.top/gtswerimrg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yangfankeji.com/gtwsbswaci.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gthwqitrgo.html

Py:   s[::-1]
来源：http://hz.xylfe.cn/gthtmxcgio.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtxvzogcxd.html

JS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtfpyvajhi.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtbeulwpix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nwbrower.top/gtpdtvakne.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jlsjyb.cn/gtyrloddul.html

Ruby: s.reverse
来源：http://hz.jyoumei.cn/gtqqqefwrx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtnhiytxqr.html

[E12] 统计某字符出现次数
来源：http://hz.sysykeji.top/gtnaeyqfig.html

Py:   s.count("a")
来源：http://hz.guannengcc.top/gtqvcdeeuk.html

PHP:  substr_count($s, "a");
来源：http://hz.snrcjt.cn/gtnbyeqrlx.html

JS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtcuvbrgav.html

TS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gtkuziorvj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.bjfxy.top/gtwhbrynig.html

Go:   strings.Count(s, "a")
来源：http://hz.snrcjt.cn/gtritapdgz.html

Ruby: s.count("a")
来源：http://hz.pycfn.com/gtlxzmeifk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gtfpkizeuh.html

[E13] 逐字符遍历
来源：http://hz.xuanzx.com/gtufyxryvu.html

Py:   for ch in s: print(ch)
来源：http://hz.xingfuxueyuan.xyz/gtvifdsrar.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtivmzqbsg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtxuzpymwu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtltnzjezq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.9152youxi.cn/gtypcopovl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gogol.net.cn/gtxpfsjevx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtkiyyzsht.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gtadyfupos.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gttirvfrog.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydzc1.top/gtxhbrpxkz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.kuanghao11.cn/gtwzolrhae.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yongpay.top/gtxblzjpqt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jyoumei.cn/gtavjjarcr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ywan-chungtsiang.top/gtnuldvrml.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.birdmap.top/gtgwmrxawa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daxiang520.top/gtispirsqe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gttqhvypzd.html

[E15] HTML 转义 / 反转义
来源：http://hz.guowangkeji.top/gtxtpkiftn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.c1oappe.top/gtlnxadtmp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yonumen.top/gtbzkffivy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.haohaochexian.top/gtfzxoszcc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydzc1.top/gtsvrmvhzn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tian-w.cn/gtavvjiqkh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.birdmap.top/gtzxpptvpy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.iojbl.cn/gtoqrylfzp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hammf.cn/gtftspnqsw.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtnbgdbegu.html

Py:   f"{1234567:,}"
来源：http://hz.iojbl.cn/gtyiuqeadb.html

PHP:  number_format(1234567);
来源：http://hz.cheryme.top/gtljoxpdeq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtyvvlcleu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtldpxmqyf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258888.top/gtdovzuxin.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtgocpywzu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangtech.top/gtjesitkje.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtmwvbyiyv.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtzmjcnmzl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gtcxwvnujh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pycfn.com/gtliylmdro.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtvtvduqty.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtqwbqrshm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangshuangyany.cn/gtvvlzaqdo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.snrcjt.cn/gtarqpeund.html

Ruby: s.capitalize
来源：http://hz.ybcxt.top/gtlfjhiayp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gthekmeunn.html

[E18] 模板占位符替换
来源：http://hz.nwbrower.top/gtvypurkxy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.vqdsnc.cn/gtvbfrplmf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtgkcoodto.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gteouiexan.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtksvlxkem.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.quarkkingdee.top/gtbdslmmhq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daxiang520.top/gtfjnilucs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnqzz.top/gtqsbviwov.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhiwuduotai.top/gtewfdphbc.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtuxxawzpr.html

Py:   s.splitlines()
来源：http://hz.chenjidiqi.icu/gtdmmyreyj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.iojbl.cn/gtccpyvdrr.html

JS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtjisohppd.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gticowcqhp.html

Java: s.lines().toList()
来源：http://hz.gogol.net.cn/gtznrtstru.html

Go:   strings.Split(s, "\n")
来源：http://hz.fzhhl.top/gtyuvdvycx.html

Ruby: s.lines
来源：http://hz.zhiwuduotai.top/gtsxjcleuf.html

C#:   s.Split('\n')
来源：http://hz.hongshengwenyu.top/gtiyiucald.html

[E20] 判断字符串是否为空
来源：http://hz.aizwys.cn/gtnfsdlbjj.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtfejngasa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtnctzuvqg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuanzhike.top/gtuzrfjizq.html

TS:   if (s === "") {}
来源：http://hz.yangfankeji.com/gthvlsoeed.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtvqphkpvw.html

Go:   if s == "" {}
来源：http://hz.havefunace.top/gtifdklsup.html

Ruby: if s.empty?
来源：http://hz.feifeiyinyue.top/gtijefjhjf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangkeji.top/gttbvxbrro.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtknxfybfi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hywenlv.cn/gtmeesxlwl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenjidiqi.icu/gtucfuulpq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtvsvtujay.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtvseuvoot.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtvqbghjif.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtkunlrdto.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtrtjwwsco.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dashuyun.cn/gtbhxxlwaj.html

[E22] 字节长度与字符长度
来源：http://hz.zhoulong.xyz/gtkkpymlpe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtxmbrcosu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gthfiohmxk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtsgesbjvp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtbxhrhuus.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtrvazxiis.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtuuuegofl.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxinkj.top/gtlyjzdulv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jianghu66.top/gtwkcuffvk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtosqawbkg.html

F. 文件与目录
来源：http://hz.yongpay.top/gtvaidohpv.html

================================================================================
来源：http://hz.sufxvd.cn/gtazapobfx.html

[F01] 读取整个文件
来源：http://hz.yj20258888.top/gtvxhfylgn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cucudq.cn/gtglufqeer.html

PHP:  file_get_contents("a.txt");
来源：http://hz.316326.xyz/gtvyqyzvas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtjrxqjuqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cheryme.top/gtdnntmwpv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtdckmdbku.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gthvzoidma.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gttvjqlbrm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jlsjyb.cn/gtgjzdgetu.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtkbzzigyv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtdccmuqhk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.andypj.xyz/gthpfncxuk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtyqommykn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gthyuwrlbc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtlhpfgavr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gtsekvbmfg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtmanfbhmh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.havefunace.top/gturhubtfg.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtldqilnce.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sweek.top/gtphdssjor.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtjxkgmfir.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtdycjayhp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtsdyxmxvo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtdewqwlee.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gtzfqmfpso.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yangfankeji.com/gtwqpwwpuh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtosbeqnnr.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtlteswyzs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.smart0.xyz/gtvqsrzqxp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtqmulhkff.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtzyeyngco.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtzrwmugor.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jianghu66.top/gtujzjyrdv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.0kj1m.cn/gtgqcklezr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gtwvvgbsoe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shuidangran.top/gtayzsmkog.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtyqvcmpvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtcbgaqyvc.html

PHP:  file_exists("a.txt");
来源：http://hz.havefunace.top/gtncvunjcl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtnxrhimzg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtpogbgboe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtapktmzfe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.vqdsnc.cn/gtarmefibt.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtamcaceaa.html

C#:   File.Exists("a.txt")
来源：http://hz.yuxming.cn/gtkfppjihe.html

[F06] 删除文件
来源：http://hz.xylfe.cn/gtcjdgkekn.html

Py:   os.remove("a.txt")
来源：http://hz.c1oappe.top/gtoqlhlpbu.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtnwsjmxgk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtxismjwjy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtofgqtovw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtakryljrx.html

Go:   os.Remove("a.txt")
来源：http://hz.zhengqikj.top/gtczxxozeg.html

Ruby: File.delete("a.txt")
来源：http://hz.shzxlz.cn/gtirzapauo.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gtwevtukol.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gthztfabct.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.guannengcc.top/gthetexzht.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gtsyqkiusf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtrvikqrxa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gthemhqgio.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tanke756.top/gtdwquxpao.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenlongwang.top/gtbtcuudhl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtnbyrofdh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnxiangtu.top/gtljrurddk.html

[F08] 遍历目录
来源：http://hz.jinghuilouyu.cn/gtpwwikrsm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtootwulkd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtragtrjiy.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtbxrnkheh.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtlxfwckle.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtuendsrsh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xziqi.cn/gtywilamam.html

Ruby: Dir.children("dir")
来源：http://hz.wangshuangyany.cn/gtavawsmni.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtxicetman.html

[F09] 获取文件大小
来源：http://hz.jyoumei.cn/gtthiqanly.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtomouqngz.html

PHP:  filesize("a.txt");
来源：http://hz.yongpay.top/gtxwdxpscd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtgbzrlxja.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtznbsulql.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtwczbzslr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ppjwa.cn/gtwmarnewc.html

Ruby: File.size("a.txt")
来源：http://hz.haohaochexian.top/gtijmcmizo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sweek.top/gtcqdikoql.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.svipenyu.cn/gtlhbxadqb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtimnagjgs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtttleubwy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtzjlomsjv.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gtjfrvzhhs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.andypj.xyz/gtjyvwygah.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtvzbxlmak.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtzycfwipq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydzc1.top/gtnutlpnpd.html

[F11] 复制与移动文件
来源：http://hz.hongshengwenyu.top/gtgnilpuhw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtptdrdtzu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtgjzxvvmu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtpwtbgiuh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtpudzdeus.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtfdkoxcwq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtqjmiywjg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtxgcvmdwu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.52xcode.cn/gtynlqewpn.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gtuabmwslx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.0kj1m.cn/gtfgnzcksn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.iojbl.cn/gtyovlejsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.redwolf501.top/gtvjinirpv.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtojluuxfj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinyuanbaomall.cn/gtndqpjroo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtrexjuyli.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtbmzoymti.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtsowxcooh.html

================================================================================
来源：http://hz.sweek.top/gtbssmzpma.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtkehilmtt.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttodyaqyp.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtnxsreqkv.html

Py:   class User: pass
来源：http://hz.sufxvd.cn/gtiycxgwrc.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gtcsywcddj.html

JS:   class User {}
来源：http://hz.cdnleiting.top/gthqvonejf.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtcjjgfwrq.html

Java: class User {}
来源：http://hz.hywenlv.cn/gtudmugkbv.html

Go:   type User struct { Name string }
来源：http://hz.sufxvd.cn/gtucgbglan.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtrdcgdcxr.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gtyidtrukm.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtohafivnn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenjidiqi.icu/gtsctceuom.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtkhzstoey.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtzvzkbwuh.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gtiqgduwbs.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtvhjuorxj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtnkjgsyae.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cucudq.cn/gtrxifiuwu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sysykeji.top/gttdzxtung.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gtuahcxsbc.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtnpvhmhry.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtumorvtud.html

JS:   this.name = "x";
来源：http://hz.vqdsnc.cn/gtiicxqido.html

TS:   name: string = "x";
来源：http://hz.jinqigfzy.top/gtwaaunthp.html

Java: private String name;
来源：http://hz.bjfxy.top/gtvtihshys.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sufxvd.cn/gtsxmwkxka.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtrvbwydpu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gticzdfqca.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtqrmriqcq.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gtlwleuikd.html


<!-- 参考信息 -->