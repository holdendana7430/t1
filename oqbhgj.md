代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gtgbhekfvd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinghuilouyu.cn/gtyvpgkzdk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xinyue.icu/gtskarmswv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pengpengdd.cyou/gtgygrkjbf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258888.top/gtywsgkocr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gthegqfpuz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pengpengdd.cyou/gtcorzhhkh.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtqwvkmzft.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtbptzzktd.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtkhqxqqbm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtywgwiouw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxinkj.top/gtwvqxpnkc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtfxqrjfix.html

[E11] 反转字符串
来源：http://hz.sufxvd.cn/gtmdaxqyyf.html

Py:   s[::-1]
来源：http://hz.daxiang520.top/gttnsbqims.html

PHP:  strrev($s);
来源：http://hz.yueranfly.top/gtvsqcfhmh.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtjccbvcex.html

TS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtxfifjxmx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yvedp.cn/gtuaixarmp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtvgggzely.html

Ruby: s.reverse
来源：http://hz.xuanzx.com/gtarnqrgsx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gttpygtnqe.html

[E12] 统计某字符出现次数
来源：http://hz.ivvv.top/gtrhnlgkdj.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gtirmbssgt.html

PHP:  substr_count($s, "a");
来源：http://hz.wangshuangyany.cn/gttkwgcecl.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtbhjirixh.html

TS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtmxmceozp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtvojbylcq.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtalrykirv.html

Ruby: s.count("a")
来源：http://hz.svipenyu.cn/gteucskaif.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtbwlupsqm.html

[E13] 逐字符遍历
来源：http://hz.jiagoushi.top/gtosrxfzgw.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtrntcghjr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj202588.top/gtikiuovxk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtzjmszobw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gtiingvzlu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj202588.top/gtdechmatz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtnzyldewm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.c1oappe.top/gtvzzbtqxh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jiagoushi.top/gtaywyekvq.html

[E14] URL 编码与 Base64
来源：http://hz.zhiwuduotai.top/gttwxumstj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shangyingyoupin.top/gtnyvoysmm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtdxivyagg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gttvuxvdbj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtsqqqctyc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fzhhl.top/gtbbpvnwpw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yongpay.top/gtebbzqaiu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtxerakiyw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shzxlz.cn/gtirntmsqf.html

[E15] HTML 转义 / 反转义
来源：http://hz.nwbrower.top/gthxmkvoxh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.havefunace.top/gtogpfxlxa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ybcxt.top/gtfrrtngbj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sysykeji.top/gtxcqvowen.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.0kj1m.cn/gtnrdgoqda.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangkeji.top/gtqjcljuim.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xylfe.cn/gtceqnxreu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gtmgfckpuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtddgylqqr.html

[E16] 数字千分位
来源：http://hz.havefunace.top/gtvqhkebao.html

Py:   f"{1234567:,}"
来源：http://hz.shzxlz.cn/gtfufiraxr.html

PHP:  number_format(1234567);
来源：http://hz.chenlongwang.top/gtwvradckc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtnqgcwwxo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtfvwprsnd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtggkmwzlm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gteoasitmr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangkeji.top/gtmptcvori.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gtbgycutgy.html

[E17] 首字母大写
来源：http://hz.jqgufenzy.top/gtmktxsqjg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtuhqxicen.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtwuolhngo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gttdtunddu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtscviuxwe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.smart0.xyz/gtohcjuepz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tanke756.top/gtwsvjliqc.html

Ruby: s.capitalize
来源：http://hz.9152youxi.cn/gtreyphzcp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jyoumei.cn/gtqmacecok.html

[E18] 模板占位符替换
来源：http://hz.316326.xyz/gteiyxukto.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtwlorxrmx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtnmcyhfou.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtsfubfohr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtjeaocaki.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gzhubu.top/gtgkyzgvkk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtcgwndlzi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtwyxpffkk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydzc1.top/gtjjbcpmdk.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtyasyytup.html

Py:   s.splitlines()
来源：http://hz.ehwqpu.com/gtoysazabn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenzaomai.com/gtblcztxbv.html

JS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gteqxteash.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtywsoediy.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangkeji.top/gtfgzwewoi.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtaoxpcdmp.html

Ruby: s.lines
来源：http://hz.gaohongyu789.top/gtubrlfvlb.html

C#:   s.Split('\n')
来源：http://hz.ydjk.org.cn/gtrwuwjyqx.html

[E20] 判断字符串是否为空
来源：http://hz.zhaomingkeji.xyz/gtefwxofjz.html

Py:   if not s:
来源：http://hz.ywan-chungtsiang.top/gtecbbjoom.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gtspbhxoqj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gogol.net.cn/gtrodsrynf.html

TS:   if (s === "") {}
来源：http://hz.c1oappe.top/gtwprtzilq.html

Java: if (s.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtjzaplqpi.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtcahpcfap.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gttlmpltrb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gtwequbknu.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtntlsphlr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shzxlz.cn/gtvsaadigy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtfymuwuok.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtytohdoss.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtlxwefpta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtotgfqqcr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gaohongyu789.top/gtwzbueoqk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.birdmap.top/gtevbomtre.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fengsongda.top/gtnzrbaopk.html

[E22] 字节长度与字符长度
来源：http://hz.pycfn.com/gtkdfrrgnc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aizwys.cn/gticztvnrt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtjrebnyjz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtigklrcpe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtzeihthmc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aibaodan.cn/gtjgvhhyxq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sxryk.cn/gtcbakfewr.html

Ruby: s.bytesize;  s.length
来源：http://hz.tianlin.xyz/gtejrevjtm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangtech.top/gtnlsqrfnl.html

================================================================================
来源：http://hz.iojbl.cn/gtqzlzwoez.html

F. 文件与目录
来源：http://hz.aibaodan.cn/gtucbpyeat.html

================================================================================
来源：http://hz.guowangkeji.top/gtfdzmqwnq.html

[F01] 读取整个文件
来源：http://hz.guannengcc.top/gtuopjbqzy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenjidiqi.icu/gtxntlvoze.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuetiantiany.cn/gtamxygkvh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtspiwyoql.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtfapsextb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtreuvrszz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtwmcdipbs.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtcksotcqs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nwbrower.top/gtlxwijmtv.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gtrkpxfywn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gtuqbffvlo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gtjygaxyft.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtiakiihco.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtneekckui.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtyoutzydh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guannengcc.top/gtefqfpype.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtaviehvdt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtggpkbuhd.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtgblhnbql.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shangyingyoupin.top/gtwdpxwwas.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtxizqecsc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sxryk.cn/gtgshxhcgs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtuhocudxy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangshuangyany.cn/gtgoerjtan.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shzxlz.cn/gtzayqurkw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuanzhike.top/gtnvjobvce.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtuaelvxkn.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gtzubrdcny.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.svipenyu.cn/gtdioxholt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.birdmap.top/gtlwpimsgp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtdibtrujk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtkzqwyvmy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.9152youxi.cn/gtqfvwrdti.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yueranfly.top/gtfmlnrgyo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtrpomqsde.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gthevbcmwz.html

[F05] 判断文件或目录是否存在
来源：http://hz.snrcjt.cn/gtateylzkg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtpfoondoy.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtiuulbxuh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtgqysdvev.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gttgnubwic.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtfuekmclv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtipnkailc.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtxxvlzfwf.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258.top/gtwfkcokgb.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gtodqlfagv.html

Py:   os.remove("a.txt")
来源：http://hz.zhijiandao.cn/gtjfljwmkd.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gtrcbcuvvq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtbzfasqwv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daxiang520.top/gtmaairviz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtntemmqsh.html

Go:   os.Remove("a.txt")
来源：http://hz.hywenlv.cn/gtiluigbwd.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtkfqdaixe.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtvhjeoxrp.html

[F07] 创建目录（含多级）
来源：http://hz.sufxvd.cn/gtgbeuhblq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ehwqpu.com/gtsrnnnpwm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtvektmjjj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtckwecpzd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtibzgbido.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxinkj.top/gtcebnbgea.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtvawmathi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtdcnfymuw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gtlngjnrkz.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtidpwnkmr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gtshcrtonj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ywan-chungtsiang.top/gtiuristpa.html

JS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtnaqhvtwt.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gtrjpohmsa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtcvnhvbrj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtvsphlcam.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtnytszdsc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guannengcc.top/gtbghscrbk.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gttzfmphjf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtnkwjjabv.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtuqgbwcpq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtnipoaqbs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gttpygogxn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtgfwcprzy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cheryme.top/gtrocfeknu.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtrndeltxx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.c1oappe.top/gtqfynogzo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtszfsxepd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtahsazqka.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydzc1.top/gttnibpyoz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtmmzwumrb.html

TS:   path.extname("a.txt")
来源：http://hz.hysaishi.cn/gtkujnfjcu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shzxlz.cn/gtxcwuxfrj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtriftcvnf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtdyaxpdto.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hywenlv.cn/gtqkjyemxx.html

[F11] 复制与移动文件
来源：http://hz.zhaomingkeji.xyz/gtblzcwelo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gttsdqluyn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtntydwljv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtuxvqiowu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtownwonzw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shzxlz.cn/gttnntplws.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cqqwz.cn/gtuldkulsa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtvwqlpwpq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.meibo888.top/gtzexigcnk.html

[F12] CSV 读写
来源：http://hz.yj20258888.top/gtjjgmjwyz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtqfgqxovj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtnpszwzgm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtelnroxeb.html

TS:   // 同上
来源：http://hz.guannengcc.top/gtzzxhzamo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gaohongyu789.top/gtgzapnlwl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jianghu66.top/gtoxinsdlz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtncsbdsbr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtwwwchuji.html

================================================================================
来源：http://hz.snrcjt.cn/gtekltgnsq.html

G. 面向对象
来源：http://hz.zhengqikj.top/gtmckwwkkv.html

================================================================================
来源：http://hz.sysykeji.top/gteyuoevjh.html

[G01] 定义类
来源：http://hz.yanxiufei.cn/gtbhdtueao.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtlczohjjb.html

PHP:  class User {}
来源：http://hz.guannengcc.top/gttbballsz.html

JS:   class User {}
来源：http://hz.cqqwz.cn/gthadbgnic.html

TS:   class User { name: string = ""; }
来源：http://hz.gotoacloud.top/gtjfsqwzzh.html

Java: class User {}
来源：http://hz.yj202588.top/gtiqevrnur.html

Go:   type User struct { Name string }
来源：http://hz.zhiwuduotai.top/gtoitpqczv.html

Ruby: class User; end
来源：http://hz.52xcode.cn/gtncjawkgl.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtwkiwldbs.html

[G02] 构造函数
来源：http://hz.tian-w.cn/gtrhpmigkj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yongpay.top/gtojheuvnj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtocxycsbh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtqhfgyllc.html

TS:   constructor(public name: string) {}
来源：http://hz.cheryme.top/gtsauioouh.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gthevomhkd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhijiandao.cn/gtujeddrtz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cucudq.cn/gtuaivhald.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtiqqssgrz.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtimgdaqgg.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtzmrxtina.html

PHP:  public string $name = "x";
来源：http://hz.shangyingyoupin.top/gtfcbljuzp.html

JS:   this.name = "x";
来源：http://hz.nanxinkj.top/gtghdeyptl.html

TS:   name: string = "x";
来源：http://hz.ywan-chungtsiang.top/gtnftwemji.html

Java: private String name;
来源：http://hz.chenzaomai.com/gtsurtmiib.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.kuanghao11.cn/gtyhhijabh.html

Ruby: @name = "x"
来源：http://hz.hfpthk.cn/gtwxprypsv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtbbefuzhv.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtamcomsnv.html

Py:   def greet(self): return self.name
来源：http://hz.jyoumei.cn/gtvabaxgwv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtjejfbuxw.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtqshpzuzn.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtniemyahp.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtlqzgpmep.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtbbrqfdqh.html

Ruby: def greet; @name; end
来源：http://hz.chenlongwang.top/gtzkvllcrl.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtbpeztllg.html

[G05] 继承
来源：http://hz.hnqzz.top/gtmpmdgrry.html

Py:   class Admin(User): pass
来源：http://hz.yonumen.top/gtycgcrwvt.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtlfdagqhk.html

JS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtbyqvqhpi.html

TS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtqvpeigax.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gtxmkcawvs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtxkviexne.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtsopxyogk.html

C#:   class Admin : User {}
来源：http://hz.yuanzhike.top/gttxdtfpdw.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gthncpqdmn.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gtmxpmibdl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtgwzjouli.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gthymqqusn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtptbaveic.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtiztjibff.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtszblfxbc.html

Ruby: def greet; "admin"; end
来源：http://hz.redwolf501.top/gtuxpzlhre.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtsscilmxe.html

[G07] 调用父类方法
来源：http://hz.cashguo.top/gtxijcgkrr.html

Py:   super().greet()
来源：http://hz.jinghuilouyu.cn/gtrvsoqvle.html

PHP:  parent::greet();
来源：http://hz.xziqi.cn/gtyodpiqkt.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gteiyieyrx.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gttfxtjlqk.html

Java: super.greet();
来源：http://hz.sufxvd.cn/gtsytucgsn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gttfzcjfdp.html

Ruby: super
来源：http://hz.yuanzhike.top/gtuyrnavah.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtkumzmtgv.html

[G08] 静态方法与属性
来源：http://hz.shangyingyoupin.top/gthpynwkzy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtkwdqnskp.html


<!-- 参考信息 -->