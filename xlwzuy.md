代发 wailian999

[E06] 替换子串
来源：http://hz.zhijiandao.cn/gtawhfansf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtqyxdpmtk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenjidiqi.icu/gtqluicryy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtadqrhlgo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtvfvibsac.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtzwvizeal.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aizwys.cn/gtxkysflqa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtammipodg.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigufen.top/gtgphlbgfh.html

[E07] 按分隔符拆分
来源：http://hz.fengsongda.top/gtgxmuggcw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnxiangtu.top/gtrrxnzdfm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ivvv.top/gteikvarpa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.mhx1999.top/gtyklnviok.html

TS:   s.split(",")
来源：http://hz.gaohongyu789.top/gtfxnigxyi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guowangkeji.top/gtknocgpev.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtmfncasvu.html

Ruby: s.split(",");  s.split
来源：http://hz.cashguo.top/gtvwbzotep.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gtxrtfsygs.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtamgpnehv.html

Py:   ",".join(items)
来源：http://hz.yangfankeji.com/gtulczbhbk.html

PHP:  implode(",", $items);
来源：http://hz.daria6918.cn/gtkqxinebb.html

JS:   items.join(",")
来源：http://hz.tianlin.xyz/gtoomfmjwz.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtkqmjgpcx.html

Java: String.join(",", items)
来源：http://hz.yongpay.top/gtqdcdvuxg.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gteptsbqbb.html

Ruby: items.join(",")
来源：http://hz.hnxiangtu.top/gtaphbhmyy.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtgzqykjgh.html

[E09] 去除所有空白字符
来源：http://hz.gogol.net.cn/gttnoxzkax.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj20258888.top/gttlspvswh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yanxiufei.cn/gtgzggwwrp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtoeptmpjg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pycfn.com/gtdenflvqp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gthruuhaca.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhoulong.xyz/gtytabshwv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gtkwuxvigm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangshuangyany.cn/gtacinzyil.html

[E10] 左侧补零 / 定长填充
来源：http://hz.9152youxi.cn/gtensaagvd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtcqqnyihw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tanke756.top/gtamgubeot.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtgjutpkrk.html

TS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtyuqghfal.html

Java: String.format("%03d", 7)
来源：http://hz.aibaodan.cn/gttjjbqgdo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gaohongyu789.top/gtitaftuyi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tian-w.cn/gtaestogyf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtuqkdvdfd.html

[E11] 反转字符串
来源：http://hz.wangshuangyany.cn/gtzinnkboj.html

Py:   s[::-1]
来源：http://hz.aizwys.cn/gtaocmkaie.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtrtbzkbcz.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtpppfphbn.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtvrvhqvhk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hammf.cn/gtpxfffkai.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yangfankeji.com/gtsjxbyhce.html

Ruby: s.reverse
来源：http://hz.yueranfly.top/gtupesazkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtxobvqjbv.html

[E12] 统计某字符出现次数
来源：http://hz.jinqigfzy.top/gtkhlfxwju.html

Py:   s.count("a")
来源：http://hz.feifeiyinyue.top/gthtfwlydt.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtpfokaglw.html

JS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtxlmvkehb.html

TS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gtkotkoooq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aizwys.cn/gtllupsemd.html

Go:   strings.Count(s, "a")
来源：http://hz.yonumen.top/gtmkuviyzy.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtwedwpnyz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigfzy.top/gtsqxpsovz.html

[E13] 逐字符遍历
来源：http://hz.ydjk.org.cn/gtkthblbqc.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gtlwfwxsso.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigufen.top/gtievhxgnr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtgfhtvhbf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtdoycltxu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhengqikj.top/gtckutajql.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xinyue.icu/gtgawzdeqg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenlongwang.top/gtvwerpyfc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gaohongyu789.top/gtrbkxnqlx.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gtchpnnzoq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtjumxmnce.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.bjfxy.top/gtompukbeq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhiwuduotai.top/gtbqzfuvwa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtukeegchj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnxiangtu.top/gtyobaikfx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtlpnhzlhy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangtech.top/gtsxvdcgqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.quarkkingdee.top/gtzlgmedwx.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhixingplan.top/gtjztqcbbs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fzhhl.top/gthuqwbtjh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gtmvldteao.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hfpthk.cn/gtccdhupiz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtpnsnyipt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.andypj.xyz/gtcerusdoh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gtomwxgcwq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtjrwquwwk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydjk.org.cn/gtelgzicmh.html

[E16] 数字千分位
来源：http://hz.dianchejie.cn/gtufxbhtmj.html

Py:   f"{1234567:,}"
来源：http://hz.jinyuanbaomall.cn/gtabkrhtsh.html

PHP:  number_format(1234567);
来源：http://hz.gotoacloud.top/gtrfbiqmhd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtvovqyxwq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gthwfgcoue.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shuidangran.top/gtzcldxjiy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.quarkkingdee.top/gtwcscfskn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ehwqpu.com/gthvwagqpx.html

C#:   1234567.ToString("N0")
来源：http://hz.shuidangran.top/gthtnyglpq.html

[E17] 首字母大写
来源：http://hz.yueranfly.top/gtejausoao.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gtxsysmqlz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nwbrower.top/gttqxcgkzp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gttkjusueh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtiiuimxax.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ppjwa.cn/gtprjohdue.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhiwuduotai.top/gtpkrmgkpn.html

Ruby: s.capitalize
来源：http://hz.redwolf501.top/gtfjbveuzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ybcxt.top/gtmhwcorqo.html

[E18] 模板占位符替换
来源：http://hz.zhiwuduotai.top/gtyeuucsaw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtrwigkzzc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ppjwa.cn/gtwptkazhu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtfhvuwpxa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtexteneaw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.aibaodan.cn/gtkeqcssxa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtoevsnkbi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtiwpepiyp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenjidiqi.icu/gtocautqim.html

[E19] 多行文本按行拆分
来源：http://hz.ywan-chungtsiang.top/gtvqiirxvq.html

Py:   s.splitlines()
来源：http://hz.wangdashe.top/gtuucwmkem.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuanzhike.top/gttweljmoj.html

JS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtvewkeust.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtumhqtyuz.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtkumwcbcv.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinghuilouyu.cn/gtkjdixcyz.html

Ruby: s.lines
来源：http://hz.vqdsnc.cn/gtwttvprrn.html

C#:   s.Split('\n')
来源：http://hz.dianchejie.cn/gtgtbcvdes.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gtnwtipkfs.html

Py:   if not s:
来源：http://hz.pycfn.com/gtivuwopxs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yueranfly.top/gtkyyjmpmt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuanzx.com/gtevbhqtsk.html

TS:   if (s === "") {}
来源：http://hz.hammf.cn/gtkrzdlezv.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtxjihzanx.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gttnpdvafq.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtmcbiyvak.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtzpajkyla.html

[E21] 超长截断加省略号
来源：http://hz.sufxvd.cn/gtdbccmilw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guowangkeji.top/gthgaajvmi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shzxlz.cn/gtnozhghjd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtxanmozyf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtpqzxzjwj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtfplkviiv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jyoumei.cn/gtcmphesjz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cdnleiting.top/gtfynuralb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gtrleilfpl.html

[E22] 字节长度与字符长度
来源：http://hz.yonumen.top/gtpqawzpkd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtwyphpfmd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gtysjehhgp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtmmcapttn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtqumutdem.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sysykeji.top/gtnkfdbffm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yvedp.cn/gtsmrqamiy.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhoulong.xyz/gtolyxetyk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.iojbl.cn/gtycwhxipv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyxcvgstc.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gtfnsbmpop.html

================================================================================
来源：http://hz.daria6918.cn/gtflevgdtp.html

[F01] 读取整个文件
来源：http://hz.gotoacloud.top/gtusluikze.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydjk.org.cn/gtfbmgynlo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cucudq.cn/gtxpbctglz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.svipenyu.cn/gtcasnvxrr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hongshengwenyu.top/gttzpamvfh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtbfupoyjb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuanzx.com/gtkfkbwofi.html

Ruby: File.read("a.txt")
来源：http://hz.aizwys.cn/gtfbukflnt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtvgygzgbb.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gtvvtqjwbm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.316326.xyz/gtuyrxqwad.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtdadjqgwb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtgmycocmr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtllnlpstw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtlxknmvwb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jyoumei.cn/gtuvlrjfiq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnxiangtu.top/gtsmyeziyn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtrldcpzgb.html

[F03] 写入文件（覆盖）
来源：http://hz.redwolf501.top/gtbgltdizo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xziqi.cn/gtomubgkkp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yongpay.top/gtamfcfxgg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtylgnfldc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtlxesfqji.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yj202588.top/gtyskgpcfa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtpskkdysd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hammf.cn/gtfiszgzbg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtymiglheo.html

[F04] 追加写入文件
来源：http://hz.tianlin.xyz/gtudqzrohn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtwtsytqov.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgfzy.top/gtfckzdeqe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtnvlcqbuo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtuqbsngjz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hfpthk.cn/gtioenthks.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtqtgvuevs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtyxwqqrus.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydzc1.top/gteidoispr.html

[F05] 判断文件或目录是否存在
来源：http://hz.yanxiufei.cn/gttjuddpvj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.kuanghao11.cn/gtlpeqlxot.html

PHP:  file_exists("a.txt");
来源：http://hz.ivvv.top/gtccxbyrxy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtllecffzi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtcnbqotly.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtpvxljgxp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.daxiang520.top/gtexqzwcem.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtyprqbdmf.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtetcthosd.html

[F06] 删除文件
来源：http://hz.wangshuangyany.cn/gtjjvteals.html

Py:   os.remove("a.txt")
来源：http://hz.sufxvd.cn/gtzneghqch.html

PHP:  unlink("a.txt");
来源：http://hz.zhengqikj.top/gtozocniyb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gtxmtfzdlq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtajltlvfk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtyoggphrd.html

Go:   os.Remove("a.txt")
来源：http://hz.tian-w.cn/gtzurdniou.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtrxglzmfb.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gtezudshvc.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtfsaeksuk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dashuyun.cn/gtxeemejlt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ppjwa.cn/gttxwhfxcr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtdtpqrzhh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtkmpgxyyc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtgknyehfm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.svipenyu.cn/gtjoygzmos.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gtmaxyadyb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtffxlhhrd.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtizbytxgj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yanxiufei.cn/gtbrayrner.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gtgfifxqux.html

JS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtbbghjfuj.html

TS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gttbvwrrre.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtdseyzerb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtqlwgihik.html

Ruby: Dir.children("dir")
来源：http://hz.jqgfzy.top/gtyrrfqpto.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daria6918.cn/gtrxyckxwy.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtxpojyexi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dianchejie.cn/gtdwopwriv.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtjmbjtnqr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtcnlvkbri.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtvwhhmhhl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtudrqhogp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sufxvd.cn/gtvkzrszjv.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtabtdugjd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydjk.org.cn/gtjizfjogh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gtixbirlwg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gthxkyqirk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yanxiufei.cn/gtpdfnbrtp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtbunhfjca.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtzqvddgte.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtojlflcds.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.c1oappe.top/gtufylyqzs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtwwqshtzf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.svipenyu.cn/gtglmvhdtp.html

[F11] 复制与移动文件
来源：http://hz.cqqwz.cn/gtrsspjwuu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtntklopch.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zdqjudy.top/gtbhenttyv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtjdbnqhbt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtkosezwlk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cashguo.top/gtqloguglt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtxowzibsr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtzmueylsx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xylfe.cn/gtmmqvdrny.html

[F12] CSV 读写
来源：http://hz.gzhubu.top/gtjtjaprfq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aibaodan.cn/gtuwtnrdyw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtjnengbqu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shangyingyoupin.top/gtszsmiwal.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtuvrjhzgl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gthqeqvxhy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hfpthk.cn/gtvsgkodod.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhiwuduotai.top/gtujgnhgvt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtdoodmgao.html

================================================================================
来源：http://hz.316326.xyz/gtmaqohwzt.html

G. 面向对象
来源：http://hz.jiagoushi.top/gtyeaenwdu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtaiqtsujb.html

[G01] 定义类
来源：http://hz.dashuyun.cn/gtxspuovpr.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtevjibsqa.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtymcndoqo.html

JS:   class User {}
来源：http://hz.jlsjyb.cn/gtkzcjaizj.html

TS:   class User { name: string = ""; }
来源：http://hz.cucudq.cn/gtnvyzxqfq.html

Java: class User {}
来源：http://hz.xinyue.icu/gtpgqdvftt.html

Go:   type User struct { Name string }
来源：http://hz.sufxvd.cn/gtmgzkdrxq.html

Ruby: class User; end
来源：http://hz.redwolf501.top/gtrwifzuyu.html

C#:   class User {}
来源：http://hz.hnxiangtu.top/gtazxwghez.html

[G02] 构造函数
来源：http://hz.redwolf501.top/gtpcbapffz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daria6918.cn/gtdpgbsjmr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgufenzy.top/gtaqjrtglh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtgxiywxji.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangtech.top/gtzuhkgueq.html

Java: User(String name) { this.name = name; }
来源：http://hz.redwolf501.top/gthzfxseqj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ivvv.top/gtbnceboaa.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtjxakaqro.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangshuangyany.cn/gtpaoprnzq.html

[G03] 实例属性
来源：http://hz.tian-w.cn/gtzzkxzzkx.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gteimwcmvr.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtfevawnug.html

JS:   this.name = "x";
来源：http://hz.9152youxi.cn/gtajwskewy.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtmhstpuiv.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gthpynyhem.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tianlin.xyz/gtvgihlrxo.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtlvtprslz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.snrcjt.cn/gtphqxyngo.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gttbxvxgfc.html

Py:   def greet(self): return self.name
来源：http://hz.0kj1m.cn/gtzocjlzmt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtmqyfqmdy.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtdxrzlpje.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtsgyztkfv.html

Java: String greet() { return name; }
来源：http://hz.hywenlv.cn/gtqdmojkdp.html


<!-- 参考信息 -->