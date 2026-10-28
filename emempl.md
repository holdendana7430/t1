代发 wailian999

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtvubqkesh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.kuanghao11.cn/gtnsvwwuwz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtdrxxpgus.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtdrglfmyj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtbydtmatu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtglolhauy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sysykeji.top/gtoenynkqf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtuqimeewz.html

C#:   s.Replace("a", "b")
来源：http://hz.shangyingyoupin.top/gtiwzmpinz.html

[E07] 按分隔符拆分
来源：http://hz.zdqjudy.top/gtsdbeytrf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.aizwys.cn/gttbnpadmt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.kuanghao11.cn/gtgllfqhmw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xziqi.cn/gtblubckpg.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gtvrjyzufh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtipwuezza.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gtezivslip.html

Ruby: s.split(",");  s.split
来源：http://hz.cqqwz.cn/gtihrbnynq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj202588.top/gtlozletnm.html

[E08] 数组按分隔符合并
来源：http://hz.xuanzx.com/gtxlnatsrs.html

Py:   ",".join(items)
来源：http://hz.meibo888.top/gtzqvhtgif.html

PHP:  implode(",", $items);
来源：http://hz.jyoumei.cn/gtezsfelon.html

JS:   items.join(",")
来源：http://hz.cqqwz.cn/gtxfbubqev.html

TS:   items.join(",")
来源：http://hz.zhaomingkeji.xyz/gtfqesyjuv.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtbnuxhbmt.html

Go:   strings.Join(items, ",")
来源：http://hz.ydjk.org.cn/gtygrxxmub.html

Ruby: items.join(",")
来源：http://hz.ydjk.org.cn/gtbmixztlj.html

C#:   string.Join(",", items)
来源：http://hz.gogol.net.cn/gtthpbrmxq.html

[E09] 去除所有空白字符
来源：http://hz.feifeiyinyue.top/gtmepmrbxt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zycfv.cn/gtdqezzlci.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daria6918.cn/gtzrekajmp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtsaminpwh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtienwprdk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ybcxt.top/gtnblbjzqp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhixingplan.top/gtxdjdjxow.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gtldlddxtr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yvedp.cn/gtxfblojcz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jiagoushi.top/gtxbdwpsng.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hysaishi.cn/gtaijsrhis.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jqgufenzy.top/gtoxochbwh.html

JS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gttfmoqlao.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtfvtndvhg.html

Java: String.format("%03d", 7)
来源：http://hz.nwbrower.top/gtkuacirwp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtqquhddbh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtdlkuihxw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daxiang520.top/gtrhduagar.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtxpxejpwp.html

Py:   s[::-1]
来源：http://hz.bjfxy.top/gtcadqmwsp.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtrovfpwoq.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtorzyozay.html

TS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtholofief.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenlongwang.top/gtierahvru.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtvjuiyesa.html

Ruby: s.reverse
来源：http://hz.yangfankeji.com/gtcwyvsiiv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtfggddpvr.html

[E12] 统计某字符出现次数
来源：http://hz.tian-w.cn/gtkqsurkym.html

Py:   s.count("a")
来源：http://hz.zhengqikj.top/gtjqnwgixu.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtnjkvuzra.html

JS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gtslxkhtna.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtikdvtvaq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sweek.top/gtonlwvoex.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtbrsbeaih.html

Ruby: s.count("a")
来源：http://hz.kuanghao11.cn/gtlxhntctu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgfzy.top/gtqnwsyalj.html

[E13] 逐字符遍历
来源：http://hz.mhx1999.top/gtjcdeelpk.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gthcbpxbob.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sysykeji.top/gtkjyrckpo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtkvmrawcy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtpzezfwnv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtrjcfxday.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.svipenyu.cn/gtloogftkc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtqaoxnuhq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtolrzxguq.html

[E14] URL 编码与 Base64
来源：http://hz.wangshuangyany.cn/gtyaptrogt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtkntwnmnt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtgraeqoba.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.quarkkingdee.top/gtvyvkqhfm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj202588.top/gthrdbhbzg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.feifeiyinyue.top/gtthtuurnq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jianghu66.top/gtkmnasrrc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gotoacloud.top/gtxrfdjrlp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhongyouzk.top/gtpruptocw.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtpxybapae.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shangyingyoupin.top/gtwwupidpj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhengqikj.top/gtxffbepdv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gtswvpxmur.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hywenlv.cn/gtbszgjryn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shangyingyoupin.top/gtqldndjwr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ivvv.top/gtyrtwtyzg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtoihiiuud.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gttctpdeyq.html

[E16] 数字千分位
来源：http://hz.gaohongyu789.top/gtpsrfacwn.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtfhedoysl.html

PHP:  number_format(1234567);
来源：http://hz.pycfn.com/gtibvlecgh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gtrdppdntb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xingfuxueyuan.xyz/gtvwizpjsl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtwjjufpcb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtthqcadlk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtorrlbojz.html

C#:   1234567.ToString("N0")
来源：http://hz.zhengqikj.top/gtuvdujcim.html

[E17] 首字母大写
来源：http://hz.andypj.xyz/gtthkudzom.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtcueiduab.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gttnqionqi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtusaphypa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtiwyjpogz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hnxiangtu.top/gtvuqcgmvn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtvfyovjbs.html

Ruby: s.capitalize
来源：http://hz.yonumen.top/gtbtaovljz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258888.top/gtymujmsur.html

[E18] 模板占位符替换
来源：http://hz.ywan-chungtsiang.top/gtjijfiyym.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yongpay.top/gtukffblqp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gttjstxnph.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtafvqjkln.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtfrfxisra.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtpkahpysm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtsdrtqwng.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tanke756.top/gthulaaimr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sufxvd.cn/gtsrwerefi.html

[E19] 多行文本按行拆分
来源：http://hz.ydjk.org.cn/gtbytbufuo.html

Py:   s.splitlines()
来源：http://hz.zhixingplan.top/gtllephkci.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aibaodan.cn/gtzdfuxbgj.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtpuahzvca.html

TS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gttatdkokv.html

Java: s.lines().toList()
来源：http://hz.yj20258.top/gtjhxadlwj.html

Go:   strings.Split(s, "\n")
来源：http://hz.fengsongda.top/gtcmweltvg.html

Ruby: s.lines
来源：http://hz.jinqigufen.top/gtfmaivzhk.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangkeji.top/gtdszmkqhe.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtqgfqfaoq.html

Py:   if not s:
来源：http://hz.smart0.xyz/gtvejiypfv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.kuanghao11.cn/gtekdttbmz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yanxiufei.cn/gtyvqhppqk.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gtwwhbokdo.html

Java: if (s.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtstnyngcw.html

Go:   if s == "" {}
来源：http://hz.feifeiyinyue.top/gtseumvles.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangtech.top/gtjzhwmxmr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhengqikj.top/gtppeiyziq.html

[E21] 超长截断加省略号
来源：http://hz.yj202588.top/gtlbwwjcvh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnqzz.top/gtdpureszx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.0kj1m.cn/gtffeajlss.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtyzeoyipr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gttqdnxjnw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtlmblnuaf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jlsjyb.cn/gtrgicvxcl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtybligvht.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gtbrnonfbh.html

[E22] 字节长度与字符长度
来源：http://hz.hammf.cn/gterqoifkm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.quarkkingdee.top/gtzcmsqbye.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtomsouotu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhongyouzk.top/gtadbvkdxu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtzgqnjupq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cheryme.top/gtxpgjjkjo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gtwwdjiijh.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtwmgslqsp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daxiang520.top/gtcizrupdg.html

================================================================================
来源：http://hz.xinyue.icu/gtsflgcxpq.html

F. 文件与目录
来源：http://hz.daria6918.cn/gtwubuneel.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfcekqeuq.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtlttxziai.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xinyue.icu/gtyzeqdrbl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ppjwa.cn/gtalsqoyog.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.bjfxy.top/gteuqkmulj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gthjubrdub.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtyrabjzvo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ivvv.top/gtmectcyzg.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtsukxwjjw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtxxbaqcbt.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gtfaypuszm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtehxzhazy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinghuilouyu.cn/gtvqavigab.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtoyshlmsu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtfxumybbv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtrwctiicm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.snrcjt.cn/gtpprzydqu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhixingplan.top/gtphyxerdy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgfzy.top/gtbncooeck.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtlmwyfvbp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangkeji.top/gtzchfikbw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258.top/gtigqbiidy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtrwrquvjo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtmdubbjhk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gttrhyswjx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtnvcndbnh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daxiang520.top/gtnxsiaqcw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fzhhl.top/gtajjmrmjk.html

[F04] 追加写入文件
来源：http://hz.hysaishi.cn/gtdvddzthz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pengpengdd.cyou/gtighrxedz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtmethodcm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtneaaijgf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtwbivdkyn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.iojbl.cn/gtwczdyzmg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.vqdsnc.cn/gtndhzcsuo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinyuanbaomall.cn/gtghvxhuiv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guowangkeji.top/gtzmuxzlhs.html

[F05] 判断文件或目录是否存在
来源：http://hz.hongshengwenyu.top/gtcbaakbna.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daria6918.cn/gtrzkdzbva.html

PHP:  file_exists("a.txt");
来源：http://hz.daxiang520.top/gtndfuuemx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtshrsowdq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtvkpkyess.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtxkkpulsi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtqmjofjls.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtbmeufnwx.html

C#:   File.Exists("a.txt")
来源：http://hz.ivvv.top/gtibmqjnvc.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtddhsnhsh.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gtvpxorqxs.html

PHP:  unlink("a.txt");
来源：http://hz.cheryme.top/gtxnxxooco.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtxxczhlrm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtznykvzvd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtdnumfjtd.html

Go:   os.Remove("a.txt")
来源：http://hz.yuxming.cn/gtxpytzdfv.html

Ruby: File.delete("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtwomwcjdw.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gtyrwpvrjj.html

[F07] 创建目录（含多级）
来源：http://hz.nanxuanxn.top/gtedbkfxye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gthtyupzlj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.0kj1m.cn/gtfdkgsfqk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtneqkwjio.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtuzhfkkxv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtjszspxji.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daria6918.cn/gtpzpomcqp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtumnccena.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jianghu66.top/gtvxdtgbcf.html

[F08] 遍历目录
来源：http://hz.gogol.net.cn/gtimdsqlhj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtvezrglih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xziqi.cn/gtstcgrtij.html

JS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtrbvoefwh.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtnferabzv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtzpgelfrf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtisssvebn.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gthvgjqqfc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ydjk.org.cn/gteunvgcnt.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtubavqoat.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtsflcsgjp.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gticrtfbfc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtaljiopwv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtdlccjysz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtyoziinyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtydhyqfhx.html

Ruby: File.size("a.txt")
来源：http://hz.hammf.cn/gtrbwhxpju.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shangyingyoupin.top/gticelnyrg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gtuopjiwpd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtvmcwuukq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtyiutrvuo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtndmjfgup.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtvtglkwnx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gtjsyirnqe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtaefsbqph.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtiwkluyzu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cqqwz.cn/gtuihkcxsj.html

[F11] 复制与移动文件
来源：http://hz.sweek.top/gtxizzvqcb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtfdgxpxto.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.snrcjt.cn/gtjrvewbmm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtkwgtwbvl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gthvdebgqm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtliqgsxtm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zdqjudy.top/gtwyxakmcv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtpoptzdoj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gtmyyudstm.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtzaradhfn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.0kj1m.cn/gteziwdblg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhiwuduotai.top/gtqojxyfyc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sxryk.cn/gtgaiylvyb.html

TS:   // 同上
来源：http://hz.ehwqpu.com/gtevtlmize.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gtqrcjcqdc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gtegxaceoc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenjidiqi.icu/gtuzbbdaml.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtlbraabfe.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdxhqzxlw.html

G. 面向对象
来源：http://hz.316326.xyz/gtrpbpdgxk.html

================================================================================
来源：http://hz.cdnleiting.top/gtbwwenfsw.html

[G01] 定义类
来源：http://hz.jqgufenzy.top/gtuvlxfozh.html

Py:   class User: pass
来源：http://hz.sweek.top/gtoiinbqrh.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gtruqxfyin.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gttoicacfo.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtsozkpgjh.html

Java: class User {}
来源：http://hz.sufxvd.cn/gtsdqlfumn.html

Go:   type User struct { Name string }
来源：http://hz.ivvv.top/gtpwzhmhin.html

Ruby: class User; end
来源：http://hz.yuxming.cn/gtwwtctlao.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtwyucgqke.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gteohfxdhu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cucudq.cn/gtbtmdwmgf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.iojbl.cn/gteqgsipxc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtmcfxggox.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigufen.top/gtioztdzah.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtaqpipiho.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangtech.top/gtflhioxgf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yvedp.cn/gtexhzkumr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sxryk.cn/gtwqstagay.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtcfmywqxb.html

Py:   self.name = "x"
来源：http://hz.xuetiantiany.cn/gtzxapdwpk.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtpuzshmwm.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gtozusdevy.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtjebisuuy.html

Java: private String name;
来源：http://hz.gotoacloud.top/gtzpuiizmy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zycfv.cn/gttxutazwz.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtqhufgava.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtbotsnwxz.html

[G04] 定义方法
来源：http://hz.ehwqpu.com/gtytgrrkeh.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtugemfplv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtarzpqjgj.html

JS:   greet() { return this.name; }
来源：http://hz.chenlongwang.top/gthpbhjarf.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtwqdbbgpd.html

Java: String greet() { return name; }
来源：http://hz.gaohongyu789.top/gtwdufkmfu.html


<!-- 参考信息 -->