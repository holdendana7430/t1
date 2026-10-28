代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.daxiang520.top/gttsteqrdq.html

Ruby: items.join(",")
来源：http://hz.redwolf501.top/gtpsnwslkf.html

C#:   string.Join(",", items)
来源：http://hz.guowangkeji.top/gtitugvjue.html

[E09] 去除所有空白字符
来源：http://hz.hysaishi.cn/gtjfbfxvrc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtgdydbxaj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtdpizybgm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtqyqaoyyl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtxzkxvlgb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuanzx.com/gtqtbrlrqj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cdnleiting.top/gtqopxwxof.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sxryk.cn/gtdcfbvbrt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.svipenyu.cn/gtckwjriyi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tanke756.top/gtadkrdjsq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenlongwang.top/gtdxdldgxo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtatkoxkrh.html

JS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtksqgagpb.html

TS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtqphivwwo.html

Java: String.format("%03d", 7)
来源：http://hz.sxryk.cn/gtgzmqlkch.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhengqikj.top/gtndhiypel.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtacrxlwri.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ppjwa.cn/gtsqgkampw.html

[E11] 反转字符串
来源：http://hz.tanke756.top/gtfnjlzpnm.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtrhyqxdfa.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtjuoxhqxa.html

JS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gttjhpnoii.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtlnjtdcme.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgfzy.top/gtkrujotia.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gteuvfrrvj.html

Ruby: s.reverse
来源：http://hz.cashguo.top/gtmqfegdbk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtdteuuuow.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtjwxmsfva.html

Py:   s.count("a")
来源：http://hz.yvedp.cn/gtsxaylmbh.html

PHP:  substr_count($s, "a");
来源：http://hz.gaohongyu789.top/gtquusleqp.html

JS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtgbxyvatk.html

TS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtqtrwohso.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.haohaochexian.top/gtiajpbpcj.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtzciuyexs.html

Ruby: s.count("a")
来源：http://hz.jqgufenzy.top/gttcannmmr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daxiang520.top/gtcnzmdmxg.html

[E13] 逐字符遍历
来源：http://hz.yanxiufei.cn/gtcqtecfov.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtkuifhcwt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yanxiufei.cn/gtlvnmjbir.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtyhgcydmu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtxljbnczg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xziqi.cn/gteyzckaod.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.52xcode.cn/gthiecxaio.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtgtbpbpyo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pycfn.com/gtlyoyzlfm.html

[E14] URL 编码与 Base64
来源：http://hz.yvedp.cn/gtsdvxgjeo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.haohaochexian.top/gtqwjeprvv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.redwolf501.top/gtpfxjwabp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtrwrmptsd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fengsongda.top/gtqsaepreq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtptpagnas.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nwbrower.top/gthfjvhtux.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhaomingkeji.xyz/gtgqtwjhbi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gtrududmuz.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtwlrfbroy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuanzhike.top/gtyhqennpp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuxming.cn/gtqwfrurii.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.svipenyu.cn/gtesattrlv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.iojbl.cn/gteycjphdm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtkshkumkw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtvthixxgt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jyoumei.cn/gtndccnxua.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shuidangran.top/gtwqgspjsj.html

[E16] 数字千分位
来源：http://hz.jyoumei.cn/gtukqaaqty.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtaygfqwdh.html

PHP:  number_format(1234567);
来源：http://hz.yuanzhike.top/gtwnrqxqqg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtqfflngwa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtgrjjikkt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenjidiqi.icu/gtmuhhjhmw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gotoacloud.top/gtdtkapvlm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gogol.net.cn/gtueiylnxb.html

C#:   1234567.ToString("N0")
来源：http://hz.xingfuxueyuan.xyz/gtytrwqbvq.html

[E17] 首字母大写
来源：http://hz.zhengqikj.top/gtcvapunyu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtgtdqhsil.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.meibo888.top/gtmpzrljeb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtipjdvgzj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shzxlz.cn/gthodluojo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jlsjyb.cn/gthaqsbcfv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgufenzy.top/gtoemssspe.html

Ruby: s.capitalize
来源：http://hz.chenlongwang.top/gtshbwokfz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cashguo.top/gtygneqybv.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtjjirwmli.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtdysqahxy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fengsongda.top/gtwhkqxeca.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gtognwlvuv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtnnwxifrl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtkgxeibpl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenzaomai.com/gtimpocbzi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtehooigfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtmxxhjjua.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gtnamrwqfm.html

Py:   s.splitlines()
来源：http://hz.jqgufenzy.top/gtmchlcxbg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtpdmvtozs.html

JS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtexbmrkqk.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtchecwbsf.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtpsysbxqi.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtytpcbama.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtlpabjdfh.html

C#:   s.Split('\n')
来源：http://hz.hammf.cn/gtdgqbmajx.html

[E20] 判断字符串是否为空
来源：http://hz.mhx1999.top/gtzqcwybmb.html

Py:   if not s:
来源：http://hz.zhengqikj.top/gtwbrotgfm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cashguo.top/gtfoazeuza.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ehwqpu.com/gtsmvyohza.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtqnzjrmfu.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtalukcyzw.html

Go:   if s == "" {}
来源：http://hz.9152youxi.cn/gtvrfsfqkj.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangtech.top/gtwquknewg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tian-w.cn/gtyoaqzbci.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangkeji.top/gtmarapjqn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aizwys.cn/gtubxpfhac.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hfpthk.cn/gtlqdqbpuz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtxqgwfhfu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtbdxanjmn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtzmfyykis.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.svipenyu.cn/gtgmmljdcb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cashguo.top/gtphvnygfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtciequowq.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtkgsqtvto.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuxming.cn/gtlixltlqo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtxmtqassg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gteieetnxp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtqwgmhwws.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.birdmap.top/gtuhhgvhro.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ybcxt.top/gtfvowmzah.html

Ruby: s.bytesize;  s.length
来源：http://hz.feifeiyinyue.top/gtvhwgzofi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gthdqtmouo.html

================================================================================
来源：http://hz.dashuyun.cn/gtqpxrmkjn.html

F. 文件与目录
来源：http://hz.xingfuxueyuan.xyz/gteafexzko.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcyxooltv.html

[F01] 读取整个文件
来源：http://hz.hammf.cn/gtqmmksozt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.kuanghao11.cn/gtbeczdold.html

PHP:  file_get_contents("a.txt");
来源：http://hz.bjfxy.top/gtgawbkwxg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gtgvgcnhqr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gttbnebzft.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtopdofsjm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnqzz.top/gteiyrmfsa.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtkestuxyy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtjnjunpzv.html

[F02] 逐行读取文件
来源：http://hz.52xcode.cn/gtmxcvmfnw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj202588.top/gtgkmmudpw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.9152youxi.cn/gtvjcdlhgw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtbptojcjb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtvjfyeavr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtpavcsqxo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhaomingkeji.xyz/gtmbypmfbr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zdqjudy.top/gtthcdeufp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guannengcc.top/gtnimcjuiy.html

[F03] 写入文件（覆盖）
来源：http://hz.jinghuilouyu.cn/gtvnjsfepl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhengqikj.top/gtgxgqzvmj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cucudq.cn/gtmkcobzpm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtystcpbvr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtzydlbxje.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtutajaifv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gttwzufhjv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.9152youxi.cn/gtnsqxxdne.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtpbcucmjx.html

[F04] 追加写入文件
来源：http://hz.hnqzz.top/gtikzlnnox.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.0kj1m.cn/gtcxzygyhe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258888.top/gtbhagjfce.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtcnppxntf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hysaishi.cn/gtwvgkhuqj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhaomingkeji.xyz/gtbcndutwb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtofssfhim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtmfxrfrta.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangtech.top/gtdarcqbds.html

[F05] 判断文件或目录是否存在
来源：http://hz.sxryk.cn/gtjyerxfoy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgfzy.top/gtafpvwxjg.html

PHP:  file_exists("a.txt");
来源：http://hz.shangyingyoupin.top/gtmwvbmyyu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtsooxnzme.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtorgroaue.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gttrjhxihz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtttzhjwsj.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxinkj.top/gttixjeaof.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtwvzbweps.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtzhhbcyjm.html

Py:   os.remove("a.txt")
来源：http://hz.fengsongda.top/gtlrencrlr.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtmziakltj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gteamobppk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtrfrwxzer.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtdchrxizg.html

Go:   os.Remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtxchauaxg.html

Ruby: File.delete("a.txt")
来源：http://hz.yueranfly.top/gtqfkissuu.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtxifeloyl.html

[F07] 创建目录（含多级）
来源：http://hz.xziqi.cn/gtvrtaalsl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtgeysqvsw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuetiantiany.cn/gttvqiikyo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtnyapjurv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gthnyvlhcb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aizwys.cn/gthkpfyqem.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtafbcrwvm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gthsyvrioe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hywenlv.cn/gtotadalda.html

[F08] 遍历目录
来源：http://hz.haohaochexian.top/gtdekyjnby.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtfrdayvig.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangshuangyany.cn/gtkunxhssm.html

JS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtpzgblsaw.html

TS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtuammtksi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtuxhdzubc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xylfe.cn/gtiwutcwsa.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtygfenzyk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtzzqipnfw.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtzmfsczzi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinghuilouyu.cn/gtiuaeavys.html

PHP:  filesize("a.txt");
来源：http://hz.hongshengwenyu.top/gtgulkubsb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gthhpmsdzc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtowtmqfjg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtlccrpvjy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtlzqqysuv.html

Ruby: File.size("a.txt")
来源：http://hz.ydzc1.top/gtwydchdbi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jyoumei.cn/gtrzjbiklz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtuglqufgx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtqefechxd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtbgjofpxj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtszucuuet.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtnqmzlygk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.havefunace.top/gtxofynhga.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtbzidljjg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtltiaxucd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jyoumei.cn/gtunlztacq.html

[F11] 复制与移动文件
来源：http://hz.tian-w.cn/gtcxrwswgc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtpxnzmeci.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gtbyhkigby.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtftehkcmw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtiyyzlhtq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cheryme.top/gtcunpdiah.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zdqjudy.top/gtdnbwdysw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtejqowxig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtpukhhdzq.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gtsghdlsgh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtinozqlba.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.snrcjt.cn/gtnsvclcrn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tianlin.xyz/gtntdpdrvv.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtzrfjssox.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.havefunace.top/gtglbpzjeq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtboirivie.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtkneagyyu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fzhhl.top/gtemirfqjt.html

================================================================================
来源：http://hz.zdqjudy.top/gtloijylgo.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtemagerpc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxocaazas.html

[G01] 定义类
来源：http://hz.birdmap.top/gtasuedkik.html

Py:   class User: pass
来源：http://hz.sysykeji.top/gtugahfepn.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtjlubtswm.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtdyzuyjlo.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gtfnmiejpc.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtprvbhtuk.html

Go:   type User struct { Name string }
来源：http://hz.gotoacloud.top/gtzstnllnd.html

Ruby: class User; end
来源：http://hz.sysykeji.top/gtclxrhepe.html

C#:   class User {}
来源：http://hz.cheryme.top/gtivcdoysw.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtxfzahkhi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gzhubu.top/gtjsucnynv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtfnqmutuv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtzavkluyd.html

TS:   constructor(public name: string) {}
来源：http://hz.sxryk.cn/gtmadszdsv.html

Java: User(String name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtnnjeeood.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtmpemhvxh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gtdgvrcktn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtjinjpham.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtipvfigzw.html

Py:   self.name = "x"
来源：http://hz.jianghu66.top/gtfgpyvpjp.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gtixiuxaoq.html

JS:   this.name = "x";
来源：http://hz.cashguo.top/gtytbtuzle.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtbdlkffgk.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtsimdbswp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtfquqzyff.html

Ruby: @name = "x"
来源：http://hz.xylfe.cn/gtigwnzqls.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gttvwdytun.html

[G04] 定义方法
来源：http://hz.fengsongda.top/gtyyzvvgsf.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtqdkkcccn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtkrtfurrn.html

JS:   greet() { return this.name; }
来源：http://hz.snrcjt.cn/gtfejnzpse.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtuatstjpj.html

Java: String greet() { return name; }
来源：http://hz.hysaishi.cn/gtcretkfri.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtaumrcvyc.html

Ruby: def greet; @name; end
来源：http://hz.9152youxi.cn/gtndizqifk.html

C#:   public string Greet() => Name;
来源：http://hz.jinyuanbaomall.cn/gttlzkyhqw.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gthhpfhoni.html

Py:   class Admin(User): pass
来源：http://hz.yj20258.top/gthlgvekzk.html

PHP:  class Admin extends User {}
来源：http://hz.haohaochexian.top/gtvkizradv.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gthpakgswc.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtxbabmjjj.html

Java: class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtoajhbprn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtwxupdigz.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtkpdsloom.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtajcoubzn.html

[G06] 重写方法
来源：http://hz.meibo888.top/gtwkraepgp.html

Py:   def greet(self): return "admin"
来源：http://hz.havefunace.top/gtyifzrhlb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gthznlibtm.html

JS:   greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtfzjujnye.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gthoiicapj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtgrdxjcku.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jyoumei.cn/gtpvcfapia.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtvnhgzqdb.html

C#:   public override string Greet() => "admin";
来源：http://hz.ivvv.top/gtdhqfzdvl.html

[G07] 调用父类方法
来源：http://hz.yonumen.top/gtrlgyaxkl.html

Py:   super().greet()
来源：http://hz.0kj1m.cn/gtjdcppyjg.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtdzizgwvq.html


<!-- 参考信息 -->