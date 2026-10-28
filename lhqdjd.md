代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.redwolf501.top/gtihwapgck.html

[E07] 按分隔符拆分
来源：http://hz.sysykeji.top/gtcmppbiqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pycfn.com/gtnistfonf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hammf.cn/gtebuvuzzu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.mhx1999.top/gtqnhmoteu.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gtnddteway.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhixingplan.top/gtprftpfkq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hongshengwenyu.top/gtbhczhgzi.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gtqcduhril.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guannengcc.top/gtwzsvezpo.html

[E08] 数组按分隔符合并
来源：http://hz.tianlin.xyz/gtvpykgspe.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtrnpnitam.html

PHP:  implode(",", $items);
来源：http://hz.guowangkeji.top/gtanlztlgl.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtgyyyxbjb.html

TS:   items.join(",")
来源：http://hz.c1oappe.top/gtgpujpiia.html

Java: String.join(",", items)
来源：http://hz.yj202588.top/gtxtazsvln.html

Go:   strings.Join(items, ",")
来源：http://hz.chenzaomai.com/gtrtcvfxfv.html

Ruby: items.join(",")
来源：http://hz.birdmap.top/gtvympkush.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangtech.top/gthtshukwa.html

[E09] 去除所有空白字符
来源：http://hz.sxryk.cn/gtmozjzozf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hnqzz.top/gtutjajled.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xziqi.cn/gtrtxmwagm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtyciqoptz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtcqcineoe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yongpay.top/gtersiivet.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinghuilouyu.cn/gtmourthsp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtcirtpjtg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenjidiqi.icu/gtavkvtkju.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtnorxgspt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ppjwa.cn/gtjfgbpfce.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtrrdrfzci.html

JS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gttzkweong.html

TS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtrbbhnlhn.html

Java: String.format("%03d", 7)
来源：http://hz.quarkkingdee.top/gtzutrlnsw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtdbddtvrl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shuidangran.top/gtncbykgay.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhixingplan.top/gtysqfffib.html

[E11] 反转字符串
来源：http://hz.quarkkingdee.top/gtqvtscpkc.html

Py:   s[::-1]
来源：http://hz.yj20258.top/gtlrcslcdv.html

PHP:  strrev($s);
来源：http://hz.316326.xyz/gtyfrxjrtb.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtdtqhyuce.html

TS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtujkpxudh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daxiang520.top/gttcdrgodk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jqgufenzy.top/gtzpvyvrda.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtupmwfyfl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtmaoxidan.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtxspjazvx.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtjjvjhciq.html

PHP:  substr_count($s, "a");
来源：http://hz.hywenlv.cn/gtcbzfflik.html

JS:   s.split("a").length - 1
来源：http://hz.shzxlz.cn/gtnbslxspq.html

TS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtzozdkcew.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.bjfxy.top/gtugkfutnd.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtdthaeqio.html

Ruby: s.count("a")
来源：http://hz.hfpthk.cn/gthrnjgsmp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtjjzfizwu.html

[E13] 逐字符遍历
来源：http://hz.fengsongda.top/gtrkgosudq.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigufen.top/gtcfceoeke.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.meibo888.top/gthhqixqll.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtgqacnspc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daria6918.cn/gtxfmojxeo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxuanxn.top/gtitastbwd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sufxvd.cn/gtkejddvlu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sweek.top/gtjbxzpjgy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zdqjudy.top/gttnjbblgf.html

[E14] URL 编码与 Base64
来源：http://hz.ybcxt.top/gthdksnilr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydjk.org.cn/gtmhiicgcx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtiwoprkjf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gtchisljky.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhixingplan.top/gtufqrgtnj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tian-w.cn/gtwhjhrgpx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cheryme.top/gtdptwiiyk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtjrvekcqf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtdxcusooq.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gtytenxubz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.9152youxi.cn/gtnuakpmbt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gaohongyu789.top/gttxygtgkr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuanzx.com/gtnaygcxxr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtrrtppnud.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.9152youxi.cn/gtzpvqdomu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.316326.xyz/gtyoztlgyz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhixingplan.top/gtwnwqbtjz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daxiang520.top/gtlwculvdm.html

[E16] 数字千分位
来源：http://hz.chenjidiqi.icu/gtizscndwj.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtoimulszw.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtkqbgwypg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtcijaugfv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtzdltmlst.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtsvaetdgn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuxming.cn/gtfatfupzp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.c1oappe.top/gtvlrunzxq.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtocwrofpx.html

[E17] 首字母大写
来源：http://hz.snrcjt.cn/gtxgfjupan.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgfzy.top/gtnnegjqch.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtxvmlqdfs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtoduchcmr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gtykcuqwcp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xziqi.cn/gtxpyueifq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtwtatqtop.html

Ruby: s.capitalize
来源：http://hz.pycfn.com/gtoxupwfyy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gtweifllwm.html

[E18] 模板占位符替换
来源：http://hz.ydjk.org.cn/gtukjyccms.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuxming.cn/gtyujjkpgj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gtexzeqvew.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtxcstnply.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtocktnabw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuxming.cn/gttcqxpqst.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aibaodan.cn/gtqvoqmeem.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cheryme.top/gtadcemksc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtpdtsmfzw.html

[E19] 多行文本按行拆分
来源：http://hz.shuidangran.top/gtjdrqenzz.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gttnipkgzd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuanzx.com/gtmfosezhr.html

JS:   s.split(/\r?\n/)
来源：http://hz.sufxvd.cn/gtlcztqjgr.html

TS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtmrpzeaei.html

Java: s.lines().toList()
来源：http://hz.redwolf501.top/gtfakqwgkh.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtzqzegjnh.html

Ruby: s.lines
来源：http://hz.quarkkingdee.top/gtiafozmrg.html

C#:   s.Split('\n')
来源：http://hz.ybcxt.top/gtuptgxsdo.html

[E20] 判断字符串是否为空
来源：http://hz.ehwqpu.com/gtzzcrsmtb.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gtpdbxgkdr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.redwolf501.top/gtfakkvepk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtkkjbqcik.html

TS:   if (s === "") {}
来源：http://hz.yuxming.cn/gtlbwrlhpn.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangdashe.top/gtuvqqkvfo.html

Go:   if s == "" {}
来源：http://hz.kuanghao11.cn/gtwpdzyyln.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtzycdsqxm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tian-w.cn/gtnlzplsgd.html

[E21] 超长截断加省略号
来源：http://hz.jyoumei.cn/gtbmjavmpj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangshuangyany.cn/gtzxnqccin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtielkxeto.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtosbdcjui.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtlxcdpvsp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtlsfcdele.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gtgwubuzpg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtiylkbuei.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cdnleiting.top/gtpkheluqc.html

[E22] 字节长度与字符长度
来源：http://hz.xinyue.icu/gtliwolfns.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gtutyebfgf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gthppkdpzd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ivvv.top/gtahwplmqc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtvvckgqev.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtceypsvaf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhoulong.xyz/gtqinstmuc.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtevmlylok.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtbjctfwsc.html

================================================================================
来源：http://hz.tian-w.cn/gtyubbxedx.html

F. 文件与目录
来源：http://hz.cdnleiting.top/gtggggnshy.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnkvznipb.html

[F01] 读取整个文件
来源：http://hz.yonumen.top/gtmrxuotzi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jianghu66.top/gtajqtuoph.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtxfdwfyik.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hongshengwenyu.top/gtawmlrzlf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cdnleiting.top/gtneermvci.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtgqpnpwyv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtqwavnjjd.html

Ruby: File.read("a.txt")
来源：http://hz.cqqwz.cn/gtijpdgadd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangdashe.top/gtghxhhneh.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gttbidgrkx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gtrrkywotk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtpmafqenp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtlfqkhojn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtzsvrkuha.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtwuqilcia.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtdoyylwqr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jianghu66.top/gtglsxblve.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtohprssoq.html

[F03] 写入文件（覆盖）
来源：http://hz.daxiang520.top/gtgaaevhjl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gthzuslonm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gteuwfidmb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daxiang520.top/gtycnelada.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtdphgglik.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtxvwqxkgp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258888.top/gtlxptkcel.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtasvmqsph.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtdxebxcfw.html

[F04] 追加写入文件
来源：http://hz.xylfe.cn/gtuogfpycf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtrxwcsnfr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtyrxrnbgg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtwredbxzp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtjcomxoxj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ybcxt.top/gtrigagmes.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnxiangtu.top/gtidvjjsgx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtxxwelobx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydzc1.top/gtfupazuwx.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gtdrdxfzpe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ivvv.top/gtqhtozyrh.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtltiyxbhc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtctrczrdm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtfvhnzngs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtytknkpkc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hongshengwenyu.top/gtbamfrvde.html

Ruby: File.exist?("a.txt")
来源：http://hz.c1oappe.top/gtonlcnrim.html

C#:   File.Exists("a.txt")
来源：http://hz.sweek.top/gtythqrtlr.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gtajocnbkh.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gthhmazeyj.html

PHP:  unlink("a.txt");
来源：http://hz.sxryk.cn/gteufjwywp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigufen.top/gtsipddfct.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtkfotzhmy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtaggdzank.html

Go:   os.Remove("a.txt")
来源：http://hz.yj20258888.top/gtolwkmrxy.html

Ruby: File.delete("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtgnbxqbzm.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtseyleyxp.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtpvfwqqtw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnqzz.top/gtexukyjxr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhongyouzk.top/gtbxiyyhtt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtncsqtxhk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258.top/gtjagjpsuk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtypbrhqtp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zdqjudy.top/gtsuqxpggo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuanzhike.top/gtdztkgrhh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gtbiaxaxkk.html

[F08] 遍历目录
来源：http://hz.zycfv.cn/gtgwazzrmy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtluokzcew.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtjkpwudmh.html

JS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtdduvxvhu.html

TS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtbrweqrqc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtjacsushv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hammf.cn/gtvtweuebl.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtrtdtkmrz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigfzy.top/gtbnurfiwm.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gtelxsejcg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhijiandao.cn/gtfazqdora.html

PHP:  filesize("a.txt");
来源：http://hz.xziqi.cn/gtsymkbthe.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtavjnrjzd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtwqjcvqti.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtubfvwvib.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtmuyxzjhe.html

Ruby: File.size("a.txt")
来源：http://hz.cheryme.top/gtdbrrbqjd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtpnkhtlpd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.vqdsnc.cn/gtidxbjrfn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtxcdkcyxm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yueranfly.top/gtqormphld.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtutdvraiv.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gtfogisqng.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtgagshpkc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtuilkdknn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtbapchcvv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gthlfkovrm.html

[F11] 复制与移动文件
来源：http://hz.ehwqpu.com/gtweiksdii.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtxpxmjxxs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gthqkrvjvt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtdudgyybf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtkfijlocb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtgvsdxeqm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtachvzwvy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtpsqoezji.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtmivvetaj.html

[F12] CSV 读写
来源：http://hz.c1oappe.top/gtkneeehnl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cucudq.cn/gtgclxgmhm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gteudnqsho.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.svipenyu.cn/gtpopfmjfq.html

TS:   // 同上
来源：http://hz.pycfn.com/gtszkbrolm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangkeji.top/gtzgxqxhrc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtkvpwdmmo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gthoipohgc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.iojbl.cn/gtbqntkvwn.html

================================================================================
来源：http://hz.dashuyun.cn/gtbwiukitz.html

G. 面向对象
来源：http://hz.jianghu66.top/gtfzrfirca.html

================================================================================
来源：http://hz.bjfxy.top/gtwebjxqua.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtffgbsbxy.html

Py:   class User: pass
来源：http://hz.jyoumei.cn/gtyuriucrj.html

PHP:  class User {}
来源：http://hz.sweek.top/gtcaovtiay.html

JS:   class User {}
来源：http://hz.316326.xyz/gthxerwgjt.html

TS:   class User { name: string = ""; }
来源：http://hz.9152youxi.cn/gtrkcomcjq.html

Java: class User {}
来源：http://hz.xuanzx.com/gthgbbuxdg.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtunhknvfg.html

Ruby: class User; end
来源：http://hz.xylfe.cn/gtmicdvpdt.html

C#:   class User {}
来源：http://hz.hnxiangtu.top/gtitgbuemu.html

[G02] 构造函数
来源：http://hz.birdmap.top/gtbflaxgsa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gttocjfgzu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtkucodcpb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtnfteckpq.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtqmvfciej.html

Java: User(String name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtralpftlb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtgkjsixsq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jlsjyb.cn/gtwgrakdrt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtlqnlnqkh.html

[G03] 实例属性
来源：http://hz.zycfv.cn/gtcagaguhp.html

Py:   self.name = "x"
来源：http://hz.daxiang520.top/gthegmatnx.html

PHP:  public string $name = "x";
来源：http://hz.jiagoushi.top/gtevdpqgcm.html

JS:   this.name = "x";
来源：http://hz.jqgufenzy.top/gtqfljibzm.html

TS:   name: string = "x";
来源：http://hz.birdmap.top/gtqftxandp.html

Java: private String name;
来源：http://hz.guowangkeji.top/gtgwxldvav.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.vqdsnc.cn/gtosmznxwc.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtyefuyxfq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtgtlrkyhc.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtfnyvyonr.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtbwaqrefx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtqbbcgrfx.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtdebmqkfc.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtlopcxwln.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtekgocqfy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.9152youxi.cn/gtcuqatquh.html

Ruby: def greet; @name; end
来源：http://hz.9152youxi.cn/gtfzvlprvj.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtgpvhllyb.html

[G05] 继承
来源：http://hz.jiagoushi.top/gtndllejpb.html

Py:   class Admin(User): pass
来源：http://hz.hysaishi.cn/gtjgwysoql.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gtjuipjode.html

JS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtbyrbeven.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtdghqxvuc.html


<!-- 参考信息 -->