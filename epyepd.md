代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.zhoulong.xyz/gtqgwvxplw.html

[E07] 按分隔符拆分
来源：http://hz.jiagoushi.top/gtyhxfjubs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gtxagzqliw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtrzigkmvk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cucudq.cn/gtkumtnrbe.html

TS:   s.split(",")
来源：http://hz.snrcjt.cn/gtuifrfvvl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sxryk.cn/gttafxebdo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.316326.xyz/gtpdlykpdy.html

Ruby: s.split(",");  s.split
来源：http://hz.snrcjt.cn/gtegucyjjw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.vqdsnc.cn/gtbzuezfed.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gtjpepyevo.html

Py:   ",".join(items)
来源：http://hz.hfpthk.cn/gtgojgizuo.html

PHP:  implode(",", $items);
来源：http://hz.gotoacloud.top/gtplnbrbrq.html

JS:   items.join(",")
来源：http://hz.mhx1999.top/gtpqguwnfl.html

TS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gtglqemgrn.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtfijhttru.html

Go:   strings.Join(items, ",")
来源：http://hz.fengsongda.top/gtbhbkaoyp.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gttvcfvtjx.html

C#:   string.Join(",", items)
来源：http://hz.pycfn.com/gtkyalbibw.html

[E09] 去除所有空白字符
来源：http://hz.yuxming.cn/gtqkfycifw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhiwuduotai.top/gtjwpurtdr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.vqdsnc.cn/gtrzaxkqhz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtaqidkdwf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jiagoushi.top/gtvyogjbbf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtcokdlrdd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhijiandao.cn/gtdyrcacad.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shzxlz.cn/gtrflsccao.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtvvmbbxdp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgufenzy.top/gtrdltlltj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gtiflohsec.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtuecctqih.html

JS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtltyzflam.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtxlkmfgus.html

Java: String.format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtkmxooeae.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sufxvd.cn/gtgfkfzgve.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.andypj.xyz/gtyzxeqfzk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnqzz.top/gtdcylykvw.html

[E11] 反转字符串
来源：http://hz.pengpengdd.cyou/gterkyudez.html

Py:   s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtelrtomep.html

PHP:  strrev($s);
来源：http://hz.iojbl.cn/gtplgyyryd.html

JS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtfiuhhtnm.html

TS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtosuvuhyk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258888.top/gtjcrzfiwq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gttpxqczvr.html

Ruby: s.reverse
来源：http://hz.sxryk.cn/gtlolxgqpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.c1oappe.top/gthylfkdce.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtouqrsrhu.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtvgutpykl.html

PHP:  substr_count($s, "a");
来源：http://hz.ydjk.org.cn/gtendjckeq.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtvzbiqgqq.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtgeponxot.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ywan-chungtsiang.top/gtjgdtqcgz.html

Go:   strings.Count(s, "a")
来源：http://hz.shzxlz.cn/gtjrbgbtfh.html

Ruby: s.count("a")
来源：http://hz.hongshengwenyu.top/gtxmfzdngb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.52xcode.cn/gtmhvkjsnw.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtipajiiot.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtrbcwvgsf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.redwolf501.top/gtmnkedglt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtyvyqhcxo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ybcxt.top/gtroqsddoe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gtsxyfpbrr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xinyue.icu/gtabbwlosy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.vqdsnc.cn/gtofwjdibg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pycfn.com/gtuwsvdioh.html

[E14] URL 编码与 Base64
来源：http://hz.zhixingplan.top/gtrnsrckbu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtfcjwvnou.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.52xcode.cn/gtthdqogen.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cqqwz.cn/gtwgxmzkjo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnxiangtu.top/gtxwzjpnhr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnqzz.top/gtpqlfbixa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.316326.xyz/gtzlutxade.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gttdpaknsb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtmavprtbv.html

[E15] HTML 转义 / 反转义
来源：http://hz.kuanghao11.cn/gtrhcowrjv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigfzy.top/gtosdiijnz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtczoqnlvl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gtvpkccoun.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258.top/gtiiiptgii.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cucudq.cn/gtonudrycb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhijiandao.cn/gtpwxzkgdv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigufen.top/gtrudinhqb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.haohaochexian.top/gtoeyyqups.html

[E16] 数字千分位
来源：http://hz.yueranfly.top/gtjrdabgbr.html

Py:   f"{1234567:,}"
来源：http://hz.jianghu66.top/gttxaccwhj.html

PHP:  number_format(1234567);
来源：http://hz.nwbrower.top/gtxizluhua.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtfbdrcnfo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtlqaztgsy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pengpengdd.cyou/gtebpcmtox.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtwwmimhbt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtwqxvepbq.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gtljueigio.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gtexyuukeh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cdnleiting.top/gtnzdcuwkt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtvophoayw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtulineayc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtslefxelh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtkhsvkbdf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ehwqpu.com/gtmljmugmx.html

Ruby: s.capitalize
来源：http://hz.vqdsnc.cn/gtazucltqr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.iojbl.cn/gtxzqhpsam.html

[E18] 模板占位符替换
来源：http://hz.smart0.xyz/gthavhngef.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtodpdwtzv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gotoacloud.top/gtrbgrxygb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtxfmnuugk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtldoaqabu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtyexqllno.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yanxiufei.cn/gtddmkijdk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinghuilouyu.cn/gtlkgyudta.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.vqdsnc.cn/gtbtjnalro.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtnlzgdnqr.html

Py:   s.splitlines()
来源：http://hz.hywenlv.cn/gtqneeuinp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gthmzljbku.html

JS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtwrhqaqil.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtcknlnxyo.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtxivginhs.html

Go:   strings.Split(s, "\n")
来源：http://hz.nwbrower.top/gtaimqxzyf.html

Ruby: s.lines
来源：http://hz.zdqjudy.top/gttmtsibxq.html

C#:   s.Split('\n')
来源：http://hz.tanke756.top/gtsyywhdmf.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtdrymgbdf.html

Py:   if not s:
来源：http://hz.yj202588.top/gtqyzvlxen.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtqoefahcg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jlsjyb.cn/gtbglwxmkv.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtjcerhzrp.html

Java: if (s.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtrkpbuvio.html

Go:   if s == "" {}
来源：http://hz.zhaomingkeji.xyz/gtyaiijhkp.html

Ruby: if s.empty?
来源：http://hz.tianlin.xyz/gtvcfjjcye.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zdqjudy.top/gtakoyfpld.html

[E21] 超长截断加省略号
来源：http://hz.jqgufenzy.top/gtjhobhzuv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtlhfrqnup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gtccbbrtrl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtbfnpbpsh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtqfnlybik.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtjtlivgiu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zdqjudy.top/gtfhfmgznl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hfpthk.cn/gtanxjqata.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.quarkkingdee.top/gtzajnxgzd.html

[E22] 字节长度与字符长度
来源：http://hz.nanxinkj.top/gtozhsntiq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtauiescnk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gtcqsqozef.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtfnvvbbcr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtsbrfmpky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hysaishi.cn/gtsvdfjayu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cashguo.top/gtyofdumtp.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgfzy.top/gtuwftrhjz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daxiang520.top/gttogicwhx.html

================================================================================
来源：http://hz.wangdashe.top/gtqxxrxiqt.html

F. 文件与目录
来源：http://hz.haohaochexian.top/gtwulijtaz.html

================================================================================
来源：http://hz.cashguo.top/gtrgyanpvb.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtuyrvaprh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gttuxgodho.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtiwkeqald.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shzxlz.cn/gtcijrvuir.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shuidangran.top/gtiyxhhuzp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gttvdjxiak.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtuqsayhwn.html

Ruby: File.read("a.txt")
来源：http://hz.shangyingyoupin.top/gtroqcpkqv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtruhbpuzx.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtzgeqibhe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shuidangran.top/gtnfgbcrwj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tanke756.top/gtviywlbaq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtgskcqsjt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gtnzifzwgp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtqxoxiqlr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gtgibryzsn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zycfv.cn/gttoohnliy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sysykeji.top/gtbzadmjoq.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtynqzdvgz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ivvv.top/gtnnuxrujf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.c1oappe.top/gtxnwwpfqv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gtyuqdrsii.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtywtwnzdr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtnfhpufiw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtyxwtreel.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fzhhl.top/gtsxtmtlsu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangkeji.top/gtmebdgxmw.html

[F04] 追加写入文件
来源：http://hz.ywan-chungtsiang.top/gtlldceumc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gzhubu.top/gtvusdnuca.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtbkqzopwp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gthxwtgnfn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gttpbywjoh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenlongwang.top/gtlunnsega.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinghuilouyu.cn/gtauovegom.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dashuyun.cn/gtwooffavt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258.top/gtzzveuytf.html

[F05] 判断文件或目录是否存在
来源：http://hz.cheryme.top/gttpqleklq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xziqi.cn/gtuozurdpr.html

PHP:  file_exists("a.txt");
来源：http://hz.shangyingyoupin.top/gtihlwpbrk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtraxgawqz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtjbeseeiy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtlrficclb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.snrcjt.cn/gtbojpsaid.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhengqikj.top/gtpjmtyykw.html

C#:   File.Exists("a.txt")
来源：http://hz.zhoulong.xyz/gtdkokuzwf.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtaflyfmpd.html

Py:   os.remove("a.txt")
来源：http://hz.gzhubu.top/gtefalgrpb.html

PHP:  unlink("a.txt");
来源：http://hz.yongpay.top/gtvucnadfq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtatqwxgxl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtyvcgrrvt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtaysqqdsi.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgfzy.top/gtmwzmvzqb.html

Ruby: File.delete("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtefbsdibg.html

C#:   File.Delete("a.txt");
来源：http://hz.chenlongwang.top/gtmhmixfuc.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtnkpgvigk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtsqsdcxsw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cdnleiting.top/gtekrxvulw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtyceaanfp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtmhmvhuqh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gtojzahekp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sufxvd.cn/gttgnwqmqn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jianghu66.top/gtdscrtdju.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtjsijpush.html

[F08] 遍历目录
来源：http://hz.ehwqpu.com/gtythkysfe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hfpthk.cn/gtwmfcybbv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtifvgonkt.html

JS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtchfpyanv.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydzc1.top/gthxjyhqtj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gteikfrazc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zycfv.cn/gtnattzxpc.html

Ruby: Dir.children("dir")
来源：http://hz.yonumen.top/gtjtthamop.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtkfwowptm.html

[F09] 获取文件大小
来源：http://hz.shangyingyoupin.top/gtvxvsrdci.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dianchejie.cn/gtosvaqzly.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtwpdszbwo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtuvxsrjeq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtqozrcueb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtpbxndcah.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gtqfgsnjrm.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gttmfhfupg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtkgwjyhuk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yanxiufei.cn/gtjayppqlg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtcpeprzlz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtbiimpmch.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtrmctjmss.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtwzhqucgo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hongshengwenyu.top/gtgutxdrel.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtuciwtbsp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtpdkiasdy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtacrgqfrs.html

[F11] 复制与移动文件
来源：http://hz.hongshengwenyu.top/gtiaiezugo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtqobymmhd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hongshengwenyu.top/gtztdquuaf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gttciuelee.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gttxseoclb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.iojbl.cn/gtzlkuvuwh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.vqdsnc.cn/gtisqpleqp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtaccvwpjn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtyxdhtjha.html

[F12] CSV 读写
来源：http://hz.hammf.cn/gtteolpnoo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fzhhl.top/gtxptrqlta.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtxkvegkyv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gtkdpgpdeu.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtkdubhfht.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aibaodan.cn/gtfkxsvflz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtcnmsvakn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtaptcwdsf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fengsongda.top/gtbdvoufyb.html

================================================================================
来源：http://hz.sysykeji.top/gtdzcbizsr.html

G. 面向对象
来源：http://hz.zhiwuduotai.top/gtyprqygfz.html

================================================================================
来源：http://hz.haohaochexian.top/gtrazntvtx.html

[G01] 定义类
来源：http://hz.fzhhl.top/gtxkjhiapy.html

Py:   class User: pass
来源：http://hz.hywenlv.cn/gtqapbjegs.html

PHP:  class User {}
来源：http://hz.sxryk.cn/gtwmkmkufl.html

JS:   class User {}
来源：http://hz.jlsjyb.cn/gturyaucnd.html

TS:   class User { name: string = ""; }
来源：http://hz.xuanzx.com/gtrtjaorwf.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtdxxfszen.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtpjlxcbju.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtkoaypcdo.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtyrpchdwy.html

[G02] 构造函数
来源：http://hz.meibo888.top/gturokjzmi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dianchejie.cn/gtxenuzfog.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgufenzy.top/gtaaoqbmgf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtswmblqgb.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gtmolvjdqt.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtjvcxaipb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtwjcuflsi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuanzx.com/gtopiqsnee.html

C#:   public User(string name) { Name = name; }
来源：http://hz.andypj.xyz/gtivmibiys.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtjilmjlbe.html

Py:   self.name = "x"
来源：http://hz.hammf.cn/gthuaasfcc.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtpescjcto.html

JS:   this.name = "x";
来源：http://hz.jiagoushi.top/gtkcwaoosc.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtrlqknqfp.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gthlkwuika.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhoulong.xyz/gtyatxsznc.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gtvkqmykic.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangdashe.top/gtbyomvtde.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtfaadghoc.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtqyzcuyhj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtdsvvjrlt.html

JS:   greet() { return this.name; }
来源：http://hz.gaohongyu789.top/gtxriqufis.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtxwampvzp.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtomadvnxf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuanzhike.top/gtmcvcjmcv.html

Ruby: def greet; @name; end
来源：http://hz.havefunace.top/gtjdboysqg.html

C#:   public string Greet() => Name;
来源：http://hz.cheryme.top/gtllxscbrf.html

[G05] 继承
来源：http://hz.wangshuangyany.cn/gteffskstj.html

Py:   class Admin(User): pass
来源：http://hz.sweek.top/gtmyhqtlcs.html

PHP:  class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtydwcgdac.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gttlwgaspz.html

TS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gttjpetgsx.html


<!-- 参考信息 -->