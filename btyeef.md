代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtqjzgstcw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hysaishi.cn/gtyivibpxl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtxgzkxwwh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.mhx1999.top/gtfcambfgb.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtyllehqkm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgfzy.top/gtcbtnmdej.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.vqdsnc.cn/gtfoqwsxjm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtjflkguqk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtpvuqwvkd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gthbfznzoh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cucudq.cn/gttkjkdasw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenjidiqi.icu/gtzkksmkii.html

C#:   s.Replace("a", "b")
来源：http://hz.jlsjyb.cn/gtijjqfdme.html

[E07] 按分隔符拆分
来源：http://hz.cqqwz.cn/gtvsxkjlwi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtbsrijdbq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxinkj.top/gtmbnrlewg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sufxvd.cn/gthynsngow.html

TS:   s.split(",")
来源：http://hz.jinqigufen.top/gtrjdvdxik.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhengqikj.top/gteiretpet.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.9152youxi.cn/gthxoamfxf.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtfosnhlac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtkcgwyoxr.html

[E08] 数组按分隔符合并
来源：http://hz.zhaomingkeji.xyz/gtvbiwwezc.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtmzfuumdl.html

PHP:  implode(",", $items);
来源：http://hz.tanke756.top/gtvysvmqds.html

JS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtabsvrmjc.html

TS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtqwvortbz.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gtxyaunfzz.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gtrxepwjns.html

Ruby: items.join(",")
来源：http://hz.gaohongyu789.top/gtfvccflvw.html

C#:   string.Join(",", items)
来源：http://hz.zhongyouzk.top/gtqujajvan.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtxcloswlw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gtawpdebxn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtocefztwu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sufxvd.cn/gtuhlwmvjy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtydvnqhkr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.smart0.xyz/gtsllmlulh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangshuangyany.cn/gtwspatqyp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cheryme.top/gttwflnewp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtgqxobqok.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtqfkkcnsu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtxsmybgxw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtrmidvyqj.html

JS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtykngbgyr.html

TS:   "7".padStart(3, "0")
来源：http://hz.ybcxt.top/gthhhaseuj.html

Java: String.format("%03d", 7)
来源：http://hz.iojbl.cn/gtcaeywdjm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtvpcmhoxu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtaabzcrqd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tianlin.xyz/gtarrglttr.html

[E11] 反转字符串
来源：http://hz.chenjidiqi.icu/gtniqycpjt.html

Py:   s[::-1]
来源：http://hz.ydjk.org.cn/gtotscbnjf.html

PHP:  strrev($s);
来源：http://hz.ydjk.org.cn/gtlcbgpfli.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtnvwblseg.html

TS:   [...s].reverse().join("")
来源：http://hz.ybcxt.top/gthmcxsbii.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangtech.top/gtflxwhmzh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.quarkkingdee.top/gtkftlkqqu.html

Ruby: s.reverse
来源：http://hz.c1oappe.top/gtzrmhsxqx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jlsjyb.cn/gtuukgovao.html

[E12] 统计某字符出现次数
来源：http://hz.pengpengdd.cyou/gtdnqpubtz.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtemxvkxei.html

PHP:  substr_count($s, "a");
来源：http://hz.mhx1999.top/gtmmomxwva.html

JS:   s.split("a").length - 1
来源：http://hz.hfpthk.cn/gtgrzrrjma.html

TS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtgkoabinj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigufen.top/gtswvqpmal.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtpsfsdvzh.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtbqomlvfh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gtgpjqyynv.html

[E13] 逐字符遍历
来源：http://hz.andypj.xyz/gtoywrkjrz.html

Py:   for ch in s: print(ch)
来源：http://hz.shangyingyoupin.top/gtveatbgur.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zycfv.cn/gtgysfsgxo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtjpaldpnl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtqqnjeiwq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daxiang520.top/gtqklpqxfp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangkeji.top/gtqqicfdbu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daria6918.cn/gtxzkfnloh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gteelzamsz.html

[E14] URL 编码与 Base64
来源：http://hz.xingfuxueyuan.xyz/gtphhmfmyf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tian-w.cn/gtchiyggcv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydjk.org.cn/gtklkxbctn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hfpthk.cn/gtbbyqcajh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hywenlv.cn/gtyyixcunt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xinyue.icu/gtijbypffw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.9152youxi.cn/gtkrumtkgv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtdrjrbrcf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sysykeji.top/gtuutpaqdf.html

[E15] HTML 转义 / 反转义
来源：http://hz.xziqi.cn/gtwhefzggo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ehwqpu.com/gtiearehsh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtnxydkzrf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtwtecqwyp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.smart0.xyz/gtjekhnysk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuetiantiany.cn/gtxoymqoxg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtxadnfwcl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gtujeitcoz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daria6918.cn/gtmwjdesgf.html

[E16] 数字千分位
来源：http://hz.9152youxi.cn/gtsdfynwzl.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtgijqwfsu.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtjsibgtcd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtnrcyftub.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtzbzrogmz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.52xcode.cn/gtaglnmlla.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.wangshuangyany.cn/gtteucijlo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ppjwa.cn/gtizszlhkq.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtpasavcjs.html

[E17] 首字母大写
来源：http://hz.jinyuanbaomall.cn/gtrxjmxjta.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.316326.xyz/gtkqhwcmea.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtjwfyzuky.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtgossyfst.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.meibo888.top/gtslvbmetv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.feifeiyinyue.top/gterqjzwaj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtmhjeoyic.html

Ruby: s.capitalize
来源：http://hz.quarkkingdee.top/gtfrsdbvte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zycfv.cn/gtjecdaiiv.html

[E18] 模板占位符替换
来源：http://hz.dianchejie.cn/gtuqxtcyxk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.pycfn.com/gtyzudlkxw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtskpbujwg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtcimveech.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtdpyrueoj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cheryme.top/gtyaingnmc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aizwys.cn/gtinksjcrv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gteacmbbft.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dianchejie.cn/gtoynbceds.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gtegaqbtzk.html

Py:   s.splitlines()
来源：http://hz.zhixingplan.top/gtcsqfhrgg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtrrkmlzpe.html

JS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtecyhvaan.html

TS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtghpviwph.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtsyfbdudv.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinyuanbaomall.cn/gtgoxhxdhy.html

Ruby: s.lines
来源：http://hz.jinyuanbaomall.cn/gtynlminbx.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtlrqbjjar.html

[E20] 判断字符串是否为空
来源：http://hz.c1oappe.top/gtayediqea.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gtivchonwe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gtlyfsksfx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhoulong.xyz/gtfkekhrxd.html

TS:   if (s === "") {}
来源：http://hz.zycfv.cn/gttqkoxrlf.html

Java: if (s.isEmpty()) {}
来源：http://hz.hammf.cn/gtvbwztmnn.html

Go:   if s == "" {}
来源：http://hz.daxiang520.top/gtiugvyhxc.html

Ruby: if s.empty?
来源：http://hz.hammf.cn/gtfczfvotz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinyuanbaomall.cn/gtxsndnonw.html

[E21] 超长截断加省略号
来源：http://hz.tian-w.cn/gtfsrtudsj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shuidangran.top/gtovsapsce.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hongshengwenyu.top/gtjumfonjc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtpysaqbxf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtujiwhnup.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtvuaxrghp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtvpoecxka.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daria6918.cn/gtywtoehmv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yonumen.top/gtrvtgbiio.html

[E22] 字节长度与字符长度
来源：http://hz.pengpengdd.cyou/gtoasgqzpl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.feifeiyinyue.top/gtqywuccxl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhixingplan.top/gtxegduivp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtaxgifhwh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtfowlxhwv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtxqrdglbv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenlongwang.top/gtwruyuflq.html

Ruby: s.bytesize;  s.length
来源：http://hz.ywan-chungtsiang.top/gtcxdyjpmq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.snrcjt.cn/gthzyddqyx.html

================================================================================
来源：http://hz.snrcjt.cn/gtsqyihxvq.html

F. 文件与目录
来源：http://hz.yvedp.cn/gtunehyjnm.html

================================================================================
来源：http://hz.xuanzx.com/gtorsxxyct.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtacmuzydh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ywan-chungtsiang.top/gtcqqmdayc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yangfankeji.com/gtjfelttir.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtxkvlmvfn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.aizwys.cn/gtxyzyrdpy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtqjgzlwtl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtqxmqjppn.html

Ruby: File.read("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtnemfxvfe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangdashe.top/gtdkecdkxa.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtwmxkgrtm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtwqtoqzvu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj202588.top/gtjssltlqv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtkzbygvcq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtkjmolllk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtzeclvmtf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jiagoushi.top/gtgjniiwwe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ehwqpu.com/gtqchxuqes.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhijiandao.cn/gtzgqkwrwz.html

[F03] 写入文件（覆盖）
来源：http://hz.ppjwa.cn/gtyyifujcx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtiecojexk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hammf.cn/gtlwiejeaf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtbjcwbvsz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtzmlfwpyq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.snrcjt.cn/gtuegkwwsy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nwbrower.top/gtemkeavtx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuanzx.com/gtuvlxtuld.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtggqupisk.html

[F04] 追加写入文件
来源：http://hz.guannengcc.top/gtodivtrbm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sysykeji.top/gtjysldnzy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.snrcjt.cn/gtdaecjsqe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtolktbkxg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtfyoteqya.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtgrwjbtfv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtjxqffjgv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuetiantiany.cn/gtsoclsquc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.quarkkingdee.top/gthceeterz.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhijiandao.cn/gtfxgztmmg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fengsongda.top/gtgxdvmnbd.html

PHP:  file_exists("a.txt");
来源：http://hz.wangshuangyany.cn/gtxvqicfqu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtyejatfsp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtxpkmrxjv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtfpaoojhg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gtdcuyzlfv.html

Ruby: File.exist?("a.txt")
来源：http://hz.guowangkeji.top/gtywiwumcx.html

C#:   File.Exists("a.txt")
来源：http://hz.gzhubu.top/gtmneykyzc.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtjiaxyiwr.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtksecruxr.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtbxhkllsz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtxucuiyyn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtolumicmz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtqghakvmu.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gtzzedfyyf.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtfucnulzf.html

C#:   File.Delete("a.txt");
来源：http://hz.316326.xyz/gtpjtkdwum.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtylbytgxd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtlpwuzfmk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtubelbknq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtjjyupaud.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtuyabsfnn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtpynbzfzq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guowangkeji.top/gtrbrvhmgj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pycfn.com/gtrsodhlyu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yueranfly.top/gtosxtoukc.html

[F08] 遍历目录
来源：http://hz.jyoumei.cn/gtljrfvksd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtzacfclpq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gtdpdpkjjq.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtljkywtwt.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtbbkxvmlr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtubutregt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxuanxn.top/gtmbiiruzw.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gteqcyorsb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtkuezllxy.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtdtnsexcn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gtdlcqgnzk.html

PHP:  filesize("a.txt");
来源：http://hz.jyoumei.cn/gtrdmjyvfh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtxkemvdjg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtgvhvrzrh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gttoiqxbmf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhixingplan.top/gtohzosbaf.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtcecjmocz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinghuilouyu.cn/gtggqoqkam.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258.top/gtqtpwwhop.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtaamsohdo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yvedp.cn/gtofanizko.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtrryvsmuk.html

TS:   path.extname("a.txt")
来源：http://hz.ydjk.org.cn/gtnpphkrhx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuanzhike.top/gtjcfrokrv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ehwqpu.com/gtnmkxwzqb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtrspqrorn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtjjumnceq.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtucqfuqvo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtkoewzqjc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gteoshkxnl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtbrcguwuq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtxhwqihxk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtblcnkajx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.c1oappe.top/gtmgnhxiau.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtnsbppukr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gtdqsofcwm.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtssxkzscm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtpiwhokdb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtyihnclxr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnqzz.top/gtlqzjbawz.html

TS:   // 同上
来源：http://hz.ivvv.top/gtcwoayaty.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtygiwhrjy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.havefunace.top/gttfiijydj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtowuvzjmk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.0kj1m.cn/gtddbunugv.html

================================================================================
来源：http://hz.dashuyun.cn/gtdgexoxle.html

G. 面向对象
来源：http://hz.bjfxy.top/gthsnowsjv.html

================================================================================
来源：http://hz.ppjwa.cn/gtkpnqrjka.html

[G01] 定义类
来源：http://hz.feifeiyinyue.top/gtbkscrcje.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gtwdkmflgf.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtlpuaimai.html

JS:   class User {}
来源：http://hz.andypj.xyz/gttvjnzuri.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gtlmayuyou.html

Java: class User {}
来源：http://hz.jinghuilouyu.cn/gtkkkjhlme.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtajhgizyr.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gticxineys.html

C#:   class User {}
来源：http://hz.aizwys.cn/gtuoqszhbc.html

[G02] 构造函数
来源：http://hz.ydzc1.top/gtixtbiolu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gthzsgrthi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenjidiqi.icu/gtnnkcupud.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtpcznqlgt.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtrmanxfqs.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtjbmigseg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dashuyun.cn/gtmhqgkwvd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtqtywavkq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtkqyjsknz.html

[G03] 实例属性
来源：http://hz.redwolf501.top/gtzefmabmh.html

Py:   self.name = "x"
来源：http://hz.pengpengdd.cyou/gtghpkemro.html

PHP:  public string $name = "x";
来源：http://hz.aibaodan.cn/gtetkmowis.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gthikyabmg.html

TS:   name: string = "x";
来源：http://hz.ydjk.org.cn/gtxkyzzwhv.html

Java: private String name;
来源：http://hz.fengsongda.top/gtsxyqaqzd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yongpay.top/gtnobwoeuz.html

Ruby: @name = "x"
来源：http://hz.shangyingyoupin.top/gtoskrdihu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258888.top/gtevcubqwg.html

[G04] 定义方法
来源：http://hz.tian-w.cn/gtddqsikeg.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtfsfqguax.html


<!-- 参考信息 -->