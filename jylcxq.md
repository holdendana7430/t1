代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtaxisyxqk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sweek.top/gtydkaofbc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258888.top/gtubpbnjhh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xuanzx.com/gtqvkgrbcn.html

[E06] 替换子串
来源：http://hz.jinyuanbaomall.cn/gtdhwbrhwt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenzaomai.com/gtvonslpwm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cdnleiting.top/gtnsnykwoo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtvzcjvvwj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtwyfuoqvq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtiehgyezx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fengsongda.top/gtfasdpmps.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.havefunace.top/gtloeccrrk.html

C#:   s.Replace("a", "b")
来源：http://hz.ppjwa.cn/gtblmwxvqm.html

[E07] 按分隔符拆分
来源：http://hz.pycfn.com/gtqfgaxdzs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtigknjrqm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtplovagyj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangtech.top/gtyvvhqbjp.html

TS:   s.split(",")
来源：http://hz.yonumen.top/gtstcgmmjo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtcekceikf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenlongwang.top/gtzudnunks.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtoycxsfbv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ybcxt.top/gtufnbnvzi.html

[E08] 数组按分隔符合并
来源：http://hz.chenlongwang.top/gtgdlnhcpx.html

Py:   ",".join(items)
来源：http://hz.zhijiandao.cn/gthpzbigis.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gtqpjnivrv.html

JS:   items.join(",")
来源：http://hz.cheryme.top/gtggtezxkd.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gtevkmvhxk.html

Java: String.join(",", items)
来源：http://hz.haohaochexian.top/gtpqmrofpn.html

Go:   strings.Join(items, ",")
来源：http://hz.ehwqpu.com/gtpgjtbgnp.html

Ruby: items.join(",")
来源：http://hz.hywenlv.cn/gtxglgesip.html

C#:   string.Join(",", items)
来源：http://hz.yongpay.top/gtcnkcmidi.html

[E09] 去除所有空白字符
来源：http://hz.yuanzhike.top/gtrayihwpb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhaomingkeji.xyz/gtxdrnuota.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tianlin.xyz/gtzmiysobl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtitajalsc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtttzmcwxu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxinkj.top/gtgpassmsq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jyoumei.cn/gtzpcxzjed.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnxiangtu.top/gtrshnspga.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tian-w.cn/gtwhuxzhxu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.52xcode.cn/gteqtaixgr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtwpkckaaz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.smart0.xyz/gtnlrkzizd.html

JS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtqargwjoy.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtwebdlsfm.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtafcenfzf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.iojbl.cn/gttutecxlw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gtwhuxfgbz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.haohaochexian.top/gtlcxdsvdl.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gtnchkzkma.html

Py:   s[::-1]
来源：http://hz.sweek.top/gtgsiuopyh.html

PHP:  strrev($s);
来源：http://hz.hammf.cn/gthbimmnof.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtejvguqom.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtolrhenno.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhijiandao.cn/gtxrmzvama.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.daxiang520.top/gttgydjpsy.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gttlvmouuw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gthrjdbebx.html

[E12] 统计某字符出现次数
来源：http://hz.0kj1m.cn/gtvwyyztye.html

Py:   s.count("a")
来源：http://hz.yongpay.top/gtullqfqlk.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtuymsivhc.html

JS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gtptrlajow.html

TS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtvwermzwz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigufen.top/gtzvmsqbft.html

Go:   strings.Count(s, "a")
来源：http://hz.zhaomingkeji.xyz/gttvxpslku.html

Ruby: s.count("a")
来源：http://hz.tanke756.top/gttdkxthnl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gthaakjcge.html

[E13] 逐字符遍历
来源：http://hz.52xcode.cn/gtcydqkntl.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gtllusexpn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gttorxtkkp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtysluipto.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtaznimufo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj202588.top/gtlhxoshec.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.feifeiyinyue.top/gtnrctelfs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinqigufen.top/gtadrhmtfv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gtwpsysukx.html

[E14] URL 编码与 Base64
来源：http://hz.dashuyun.cn/gtdogprtur.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtrqdacnno.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.iojbl.cn/gtteltenzq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhijiandao.cn/gthrvdvqrs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj202588.top/gtvmpjidwq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gtegzptyun.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.316326.xyz/gtfhznsmrt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zdqjudy.top/gtuwyphsde.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fengsongda.top/gtzbbyjqil.html

[E15] HTML 转义 / 反转义
来源：http://hz.hywenlv.cn/gtvnnggseh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gthbktrhhe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtpfbwuphh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtxfaobssz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhengqikj.top/gtbrhgavlx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangshuangyany.cn/gthmjhncdg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.quarkkingdee.top/gtuwkpwfbb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gtiixsegdt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daria6918.cn/gtfeczzrhn.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtrejqfxlc.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtaujwfocy.html

PHP:  number_format(1234567);
来源：http://hz.hnxiangtu.top/gtbmgedxct.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtisvzucrt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtakzxhkih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhijiandao.cn/gttophgsrf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtgtuwxjyz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.vqdsnc.cn/gtbhzicbws.html

C#:   1234567.ToString("N0")
来源：http://hz.xuetiantiany.cn/gtdkvnrdrw.html

[E17] 首字母大写
来源：http://hz.shangyingyoupin.top/gtdthhtrgj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ybcxt.top/gtlefwxazf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtwrfzzryt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gthyvqmhcw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gtvrgnzchc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gtjcwqahbi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cdnleiting.top/gtsotuzawi.html

Ruby: s.capitalize
来源：http://hz.tanke756.top/gtegneqwgl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xziqi.cn/gtxrfeomgc.html

[E18] 模板占位符替换
来源：http://hz.zhaomingkeji.xyz/gtjcciiqmm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cashguo.top/gttxajtwgu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xingfuxueyuan.xyz/gtlqltldoz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtleykougy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtrznbjnpn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.316326.xyz/gteiqkzald.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shzxlz.cn/gthjsppjom.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.wangdashe.top/gtmjvypjuy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgfzy.top/gtrsgqwqli.html

[E19] 多行文本按行拆分
来源：http://hz.jinyuanbaomall.cn/gtrwfowunm.html

Py:   s.splitlines()
来源：http://hz.0kj1m.cn/gtdscloqsb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtahdgxtkv.html

JS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gtmyaexupn.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gteisomona.html

Java: s.lines().toList()
来源：http://hz.zhaomingkeji.xyz/gthxnkorss.html

Go:   strings.Split(s, "\n")
来源：http://hz.yvedp.cn/gtbxcucsdg.html

Ruby: s.lines
来源：http://hz.9152youxi.cn/gtzbkncaqv.html

C#:   s.Split('\n')
来源：http://hz.gaohongyu789.top/gtruizyiin.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtohlmfvbr.html

Py:   if not s:
来源：http://hz.tianlin.xyz/gtftsflzro.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gtxbreyvcg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gtrpumtjaa.html

TS:   if (s === "") {}
来源：http://hz.mhx1999.top/gtdzeblpkl.html

Java: if (s.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtzqptjuwt.html

Go:   if s == "" {}
来源：http://hz.ppjwa.cn/gtwvdygknq.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtuhajwzgs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gthsqiqpjf.html

[E21] 超长截断加省略号
来源：http://hz.tian-w.cn/gtmqaojteb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtgezfyzfz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dianchejie.cn/gtfvrpgwen.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtmfaqtude.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtfexchmpr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtzznhepqg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgfzy.top/gtvomwufyy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtdfmjnhge.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jiagoushi.top/gtropjqkvp.html

[E22] 字节长度与字符长度
来源：http://hz.0kj1m.cn/gtttipimtw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.316326.xyz/gtqubnxvgq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtqjxdvlvy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtnmcrhpsv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gtfvcgqpkc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinyuanbaomall.cn/gtfaviblgl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hammf.cn/gtotnwboxh.html

Ruby: s.bytesize;  s.length
来源：http://hz.yonumen.top/gtpkbkxlld.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtcttynfgu.html

================================================================================
来源：http://hz.sweek.top/gtcpcfjvba.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtnmgxsass.html

================================================================================
来源：http://hz.chenzaomai.com/gtlxlnwomf.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtnkhviqcn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuanzhike.top/gtjzlmprui.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ppjwa.cn/gtrgtgrffo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sxryk.cn/gtkixlxmmr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtubamwfhz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtvzumawbu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gtfpiyzfsq.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtrpfqkztn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.meibo888.top/gtoqwywnww.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtrpzcklxi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtvbdsdqzc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtcblrdwzz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtpfxjpmsn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gthmldohnx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtiigwdwil.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cheryme.top/gtsgfwvvms.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hammf.cn/gtitnchncc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.9152youxi.cn/gtixndpxja.html

[F03] 写入文件（覆盖）
来源：http://hz.fzhhl.top/gtbtygvcew.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhengqikj.top/gtuamhksiz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtdhkajymz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtjwmirznd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtozjlgrjp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinyuanbaomall.cn/gtajwnzyox.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aibaodan.cn/gtobsmoybi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258.top/gtbavquzxu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuanzx.com/gtgtrlclsr.html

[F04] 追加写入文件
来源：http://hz.jlsjyb.cn/gtmhikliha.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtktkrvhmb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gtgrjgqphu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtyndufbct.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtxzkrneot.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxuanxn.top/gtzjqlzlps.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gtqzgaqosb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shanyushiyangtech.top/gtptvmfnjd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gotoacloud.top/gtewyzxdpl.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnxiangtu.top/gtlxqfskbv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtoqsnqdsu.html

PHP:  file_exists("a.txt");
来源：http://hz.ybcxt.top/gtozxrughh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtvqtfxhka.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtbvxzkevi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtwqcdbftx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gthdxdkydl.html

Ruby: File.exist?("a.txt")
来源：http://hz.yanxiufei.cn/gtftegjgqu.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gtitacperx.html

[F06] 删除文件
来源：http://hz.yongpay.top/gtsfyemuys.html

Py:   os.remove("a.txt")
来源：http://hz.gotoacloud.top/gttrsjrgdl.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258.top/gtgjamwolx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtbsvazjjg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.redwolf501.top/gtdjdrtwqa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtqdhilpie.html

Go:   os.Remove("a.txt")
来源：http://hz.tianlin.xyz/gtsdegwzet.html

Ruby: File.delete("a.txt")
来源：http://hz.zhengqikj.top/gtenrvbbpn.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtigollimx.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtvewghayq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daxiang520.top/gtjtohwbyx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtxorxlmel.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shzxlz.cn/gtvecahqix.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gttupcyxkn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.iojbl.cn/gttplpobza.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hywenlv.cn/gtdbystabz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangkeji.top/gtkwosetod.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuanzhike.top/gtdpardzey.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gtracecrqn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tanke756.top/gtxyccbbtl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtzriijgih.html

JS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtebaykwld.html

TS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtgeqrywxn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aizwys.cn/gtfazkeuxd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydzc1.top/gtmdnzybon.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtheqojwgn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtrokqkobs.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtwikseuwk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.snrcjt.cn/gtcepyuwzn.html

PHP:  filesize("a.txt");
来源：http://hz.jqgfzy.top/gtbfdajblh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtkjwbnaov.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtgmibigom.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gttxixfebl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtastziuol.html

Ruby: File.size("a.txt")
来源：http://hz.sufxvd.cn/gtwngsnial.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aibaodan.cn/gtamxcesbc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gttfzmohdy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtlieluqlp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxinkj.top/gtbcbkqmxk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtflmfglpc.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtiffmvpui.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtdokgedrj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xylfe.cn/gtphiuveae.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtoxlsavnh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtejqmqgmf.html

[F11] 复制与移动文件
来源：http://hz.jlsjyb.cn/gtipfqeudt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtfkcywzsn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtuiioamju.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gttbppibtx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtdkcftyyp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtfuzhylsm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gogol.net.cn/gtswjskwhk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gttxatdjdq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gotoacloud.top/gtwhgnfvci.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gtybowxbpk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtdubdyqwr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258.top/gtcupqxknf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gthjeqagme.html

TS:   // 同上
来源：http://hz.fzhhl.top/gtbcjhxihx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.iojbl.cn/gtyngmvhog.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuetiantiany.cn/gtwwmuiiuk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtlmxzpzxb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhongyouzk.top/gtocyetmlr.html

================================================================================
来源：http://hz.jlsjyb.cn/gttlzzckqo.html

G. 面向对象
来源：http://hz.yj20258888.top/gtumwhwdwt.html

================================================================================
来源：http://hz.birdmap.top/gtbdihaysi.html

[G01] 定义类
来源：http://hz.9152youxi.cn/gtpwbdcxbq.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtlzpipfvx.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtvjnfkdtz.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtxjxxhmjw.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtcdmfalwa.html

Java: class User {}
来源：http://hz.fengsongda.top/gtkkjixunh.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtiemeovab.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtfgcljnfc.html

C#:   class User {}
来源：http://hz.birdmap.top/gtorzyphyd.html

[G02] 构造函数
来源：http://hz.pycfn.com/gttbhlaict.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtqosgwkum.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtieqhvtlf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtldbrcaoj.html

TS:   constructor(public name: string) {}
来源：http://hz.shuidangran.top/gteehvzjwb.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtqdfvuzev.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cashguo.top/gtrwnzwulu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jianghu66.top/gtvxdewlqz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtjrdqjixu.html

[G03] 实例属性
来源：http://hz.andypj.xyz/gtlqrkbbxo.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtlfgxhrut.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtreoehuqb.html

JS:   this.name = "x";
来源：http://hz.aizwys.cn/gteqyknqba.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtpdoanaef.html

Java: private String name;
来源：http://hz.smart0.xyz/gtdohinpbl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtbpgpjlja.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtkkmrsehx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gtdzayetey.html

[G04] 定义方法
来源：http://hz.sweek.top/gtldnmonbb.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtiqteqmrj.html


<!-- 参考信息 -->