代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jiagoushi.top/gtnextdilp.html

TS:   s.split(",")
来源：http://hz.yongpay.top/gtbiyooeik.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yongpay.top/gthvgbcntp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxinkj.top/gtxnxwdcea.html

Ruby: s.split(",");  s.split
来源：http://hz.0kj1m.cn/gtmdqrkwgm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shangyingyoupin.top/gticlciqus.html

[E08] 数组按分隔符合并
来源：http://hz.zycfv.cn/gttkhyiaiv.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtdrlrrsby.html

PHP:  implode(",", $items);
来源：http://hz.cheryme.top/gtaaswgnxi.html

JS:   items.join(",")
来源：http://hz.xuanzx.com/gtmbqnknhq.html

TS:   items.join(",")
来源：http://hz.gogol.net.cn/gtofiedonh.html

Java: String.join(",", items)
来源：http://hz.ehwqpu.com/gtgzonpbnc.html

Go:   strings.Join(items, ",")
来源：http://hz.zdqjudy.top/gtpnayvwiq.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtmdqtewsd.html

C#:   string.Join(",", items)
来源：http://hz.havefunace.top/gtybhcffxp.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtwqtbyjdu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtoktdwlpr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtrzeggnpa.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtoxeudmvy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtapvukdni.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtzqqrrfiq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtiplzffnc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aizwys.cn/gtfnqjmsoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pengpengdd.cyou/gtoqkvgujy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.aibaodan.cn/gtmhamtrmn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhongyouzk.top/gtuuioname.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhiwuduotai.top/gtqaefayvq.html

JS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtqvfvidfi.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenlongwang.top/gthucyoxuq.html

Java: String.format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gthdllznwp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtdzogmxkb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xinyue.icu/gtivtzeuyr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gotoacloud.top/gtufkjwjmt.html

[E11] 反转字符串
来源：http://hz.shanyushiyangtech.top/gtwgflhnhp.html

Py:   s[::-1]
来源：http://hz.aibaodan.cn/gtzcsugokv.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtqtuddeoq.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gthyhxcxlp.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtvxwwkwtn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtdpeorwti.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ywan-chungtsiang.top/gtvgkiaiyc.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtbrqfpjii.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtkgwacyih.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtybdrhhgw.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtaypvtpdi.html

PHP:  substr_count($s, "a");
来源：http://hz.haohaochexian.top/gtcayhptpp.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtffzmwohy.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangtech.top/gtoauahotv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtwldcrllk.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtfdvmsnsk.html

Ruby: s.count("a")
来源：http://hz.dianchejie.cn/gtrdamukms.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gthmjbdvps.html

[E13] 逐字符遍历
来源：http://hz.yangfankeji.com/gtzmdqupbk.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gtievvtlcm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258888.top/gtjiepmwue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtkuxsdpjp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtlpsevajt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtwqxerckx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhoulong.xyz/gtxafuhcjl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtchfvqbbo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtmlognwjw.html

[E14] URL 编码与 Base64
来源：http://hz.yongpay.top/gtterjmixt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.havefunace.top/gtpglvnxow.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxuanxn.top/gthlhlvtwz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.daria6918.cn/gtrfvetlma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtimoaoolc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhaomingkeji.xyz/gtycysfwyt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.quarkkingdee.top/gtivluyjqt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tianlin.xyz/gthvxflouh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtngzgmjoj.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtwkfadfnu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gttiliadfj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangtech.top/gttnvjmryl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenzaomai.com/gteyywkqhz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tianlin.xyz/gtfugiceqe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.0kj1m.cn/gtcgpzpyhn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.316326.xyz/gtjeuixbki.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ehwqpu.com/gtvhsaeulx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtuyzwsgrg.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gtjfazwpnn.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtphlmkhzc.html

PHP:  number_format(1234567);
来源：http://hz.shangyingyoupin.top/gtnjucdwmt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtrugwhngh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtwqkbeqpk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtpzdqrgjz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fzhhl.top/gtusfblifu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhaomingkeji.xyz/gtfamedjlh.html

C#:   1234567.ToString("N0")
来源：http://hz.bjfxy.top/gtplbfxetu.html

[E17] 首字母大写
来源：http://hz.zhaomingkeji.xyz/gtogkfwryz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ywan-chungtsiang.top/gtqxmhppga.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtutdktuda.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtaqcvwpjk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gteasucitl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sufxvd.cn/gtwmlimiov.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hfpthk.cn/gtkooibxvw.html

Ruby: s.capitalize
来源：http://hz.yanxiufei.cn/gtnlxkcxyv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxuanxn.top/gtrfdyilgf.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gtolznthyh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenjidiqi.icu/gtskleckwc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sufxvd.cn/gtjvbczsxq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtcvmcosnh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtobwsavdm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gogol.net.cn/gtpnxybycp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hysaishi.cn/gtxgvfkkcu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinghuilouyu.cn/gtozsyrdsf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgfzy.top/gtmyrkopjg.html

[E19] 多行文本按行拆分
来源：http://hz.yonumen.top/gtjrmbhobg.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gtwhyeuxxt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxinkj.top/gtgisaikqh.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtzezbsyie.html

TS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtspkgqrev.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtidbxhqhj.html

Go:   strings.Split(s, "\n")
来源：http://hz.guowangkeji.top/gtqevricpw.html

Ruby: s.lines
来源：http://hz.c1oappe.top/gtczyhzcxw.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtabiuehsj.html

[E20] 判断字符串是否为空
来源：http://hz.jianghu66.top/gtftpkiypl.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtblqdmdjk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.feifeiyinyue.top/gtykmbirwp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtqmjzuywa.html

TS:   if (s === "") {}
来源：http://hz.gzhubu.top/gtnywgyniw.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtmmuwsxjs.html

Go:   if s == "" {}
来源：http://hz.jiagoushi.top/gtwzhgaiqi.html

Ruby: if s.empty?
来源：http://hz.jqgfzy.top/gthziqitdz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xinyue.icu/gtfzbhamcy.html

[E21] 超长截断加省略号
来源：http://hz.cheryme.top/gtbffboewg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.haohaochexian.top/gtcrtkvdch.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtrsmzkdca.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtiebpwoqn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtzstspdwo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtludjcnyx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cucudq.cn/gtfltiezrf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dashuyun.cn/gtwelzjewp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinqigufen.top/gtvbcaujvu.html

[E22] 字节长度与字符长度
来源：http://hz.hammf.cn/gtinawspcx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhaomingkeji.xyz/gtdqicibpc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtqlraihbh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtgiwqspcz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtxsjtffpk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.haohaochexian.top/gtqfrfvjhb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yvedp.cn/gtcumcyvng.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangdashe.top/gtlxwbnvhy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.iojbl.cn/gtdumlgwkq.html

================================================================================
来源：http://hz.chenzaomai.com/gtdguxuirq.html

F. 文件与目录
来源：http://hz.svipenyu.cn/gtpaggczss.html

================================================================================
来源：http://hz.xylfe.cn/gtjuoxvwyl.html

[F01] 读取整个文件
来源：http://hz.kuanghao11.cn/gtlhlttadx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.andypj.xyz/gtvakqikzf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ivvv.top/gtxpjkfmqm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xuanzx.com/gtvvjyvsmi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.kuanghao11.cn/gtinajsdmd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtgqefoekg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.vqdsnc.cn/gtjlcfmbns.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtdmpkqukc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jiagoushi.top/gtkrlznqrw.html

[F02] 逐行读取文件
来源：http://hz.pycfn.com/gtnfjwgsle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ivvv.top/gtvaoahiqf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gtrawwidzk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gthccrqhdu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtrpunclyy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aizwys.cn/gtoxbeyzvo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yvedp.cn/gtmzxdagfg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydjk.org.cn/gtrkpkvdfv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtgrbrgaur.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258.top/gtlzysgtpm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258888.top/gtctwdzlqy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtfvtcrlfi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtpmauzvll.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtvqbvdoxn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtoixkqivn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dashuyun.cn/gtmezeuuvf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtvmaprbzd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtlamxtifs.html

[F04] 追加写入文件
来源：http://hz.wangdashe.top/gtuzzcupjt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.fengsongda.top/gtwvqzqoro.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gttwrikqwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtkjqawnpq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtxoywminf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.9152youxi.cn/gtrbdgqzym.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gtybxjqypw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhiwuduotai.top/gtjidkkyye.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhengqikj.top/gtguzjihpo.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gtqaggvllk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.bjfxy.top/gtmbucswkz.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtjjtxxdxg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gtsyipawps.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtugciyisw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtcppqkblz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ppjwa.cn/gtgajwhnhi.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtejycopkk.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gttzeyiszg.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtzuvlbeky.html

Py:   os.remove("a.txt")
来源：http://hz.hywenlv.cn/gtwuphrtmu.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangtech.top/gthrabaxkp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtttjarstd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigufen.top/gtecceenkr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtwnlvfczc.html

Go:   os.Remove("a.txt")
来源：http://hz.shzxlz.cn/gtvqmkhrij.html

Ruby: File.delete("a.txt")
来源：http://hz.tian-w.cn/gtomficamd.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtgnyedcmy.html

[F07] 创建目录（含多级）
来源：http://hz.chenlongwang.top/gtegpmlmqk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtbwklenzq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gtwlyltotk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtgsoaxcyo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtzswkkslo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtzsvmuyiw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtklkojwaq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cucudq.cn/gturnqdkhn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ivvv.top/gtkbrxskmw.html

[F08] 遍历目录
来源：http://hz.jiagoushi.top/gtjoalylyp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtojixodyj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258.top/gtgkwupass.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtwswltfyz.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtwdbdkeif.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtohwusjxm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daxiang520.top/gtqmfovsis.html

Ruby: Dir.children("dir")
来源：http://hz.mhx1999.top/gtvcbunhwk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtpwlvghmc.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gttrmlnusn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtvgmcyrun.html

PHP:  filesize("a.txt");
来源：http://hz.gzhubu.top/gtzjgjdspn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gttafvjhyq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtsptmcoqm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtinvkowtw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gttiofddqy.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gtpswxegjb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhixingplan.top/gtdhputkcu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtmztvbqsk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtsvfmkqrb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtsfuxrcio.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtnpvqqfsg.html

TS:   path.extname("a.txt")
来源：http://hz.sysykeji.top/gtmsqphxrx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtfijbsxvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.haohaochexian.top/gtfvsxtbin.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtbjocyrur.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gtlnxatsug.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtmjwfffbc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtshsrmzwh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sysykeji.top/gtebqgyyzo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtsdegrqzo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtgtvxpihl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hongshengwenyu.top/gtfoqavggx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtcwjjhyfk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtwactarol.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.havefunace.top/gtgnjgnzmt.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gthcjjxgcu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gtdgtowqmb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.birdmap.top/gtwggrfchk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtjtlwptlr.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtknidgdla.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jyoumei.cn/gtobcmoqsh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aizwys.cn/gtmjiarnxg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtfwnhslma.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxuanxn.top/gtrwoaclug.html

================================================================================
来源：http://hz.wangdashe.top/gtheafbavi.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtkeobejxs.html

================================================================================
来源：http://hz.pycfn.com/gtmaiuxeua.html

[G01] 定义类
来源：http://hz.wangdashe.top/gthionehxk.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtfficnzxx.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtsowfrxud.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtgexjqxjo.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtwzugdjcg.html

Java: class User {}
来源：http://hz.hywenlv.cn/gtmizaosml.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gtqoayoxmo.html

Ruby: class User; end
来源：http://hz.shuidangran.top/gtdimfbcut.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtavniujgh.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtmklyrrfl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dashuyun.cn/gtrusnfeyn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtaizssmxm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtsjxjvunx.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigfzy.top/gtrkjxrzyr.html

Java: User(String name) { this.name = name; }
来源：http://hz.yongpay.top/gtszhjpmiu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pycfn.com/gtwkncvawt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gtokwrozii.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtnllorztt.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtuzjugtya.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtshazwpkc.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtcqweinru.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtngzqqbmw.html

TS:   name: string = "x";
来源：http://hz.xingfuxueyuan.xyz/gtwtxlwfdd.html

Java: private String name;
来源：http://hz.sufxvd.cn/gtjuyklage.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtqeabidlr.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtrhqybfxa.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gttsmbkwly.html

[G04] 定义方法
来源：http://hz.cheryme.top/gttruncppd.html

Py:   def greet(self): return self.name
来源：http://hz.gaohongyu789.top/gtwdxapted.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtasesaoot.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtrcqrrcib.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtumnwjjol.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtzncqnwbp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tianlin.xyz/gtgncstgxg.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtjbjsmnrk.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtpzzooplg.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtxvciqesv.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gthejismnz.html

PHP:  class Admin extends User {}
来源：http://hz.ehwqpu.com/gtljcffdax.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtggjnksrn.html

TS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtfuedcnci.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtnerwjizm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aizwys.cn/gtfouoenzg.html

Ruby: class Admin < User; end
来源：http://hz.sysykeji.top/gtujslwiuh.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtryrpuxwn.html


<!-- 参考信息 -->