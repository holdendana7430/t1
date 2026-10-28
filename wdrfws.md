代发 wailian999

PHP:  strpos($s, "x");
来源：http://hz.zhaomingkeji.xyz/gtobrqezhy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xuanzx.com/gtjxcfensf.html

TS:   s.indexOf("x")
来源：http://hz.0kj1m.cn/gtpafdlxjm.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gttfqtcvop.html

Go:   strings.Index(s, "x")
来源：http://hz.sxryk.cn/gtxbowpkmb.html

Ruby: s.index("x")
来源：http://hz.xuanzx.com/gtrfkvjbmo.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtemwaqxvg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.andypj.xyz/gtrwcykpug.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenjidiqi.icu/gtaqniqxje.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangshuangyany.cn/gtrvexzkur.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtwywyertd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jiagoushi.top/gtwdjnpxzm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtgwzlgpjc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhixingplan.top/gttwvcxpjm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shuidangran.top/gtzxcicdqo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtyyxdxrvh.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtbmfxbaiv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhijiandao.cn/gtsagzmdic.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xingfuxueyuan.xyz/gtvtptfkvh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtrgcgkxmp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtdcelcmfh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtcjriavnm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gzhubu.top/gttsywiapo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gzhubu.top/gtzbuvujjx.html

C#:   s.Replace("a", "b")
来源：http://hz.sysykeji.top/gtvmzdqudl.html

[E07] 按分隔符拆分
来源：http://hz.hysaishi.cn/gtarnvxtts.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.0kj1m.cn/gttthfrfwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gtekodbeph.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtpvqjyrjx.html

TS:   s.split(",")
来源：http://hz.gogol.net.cn/gtjndbonef.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigfzy.top/gtuxyhhrmw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jqgfzy.top/gtnbqzsklg.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtvriosksr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nwbrower.top/gtjjnkyawl.html

[E08] 数组按分隔符合并
来源：http://hz.hysaishi.cn/gtedupwvdw.html

Py:   ",".join(items)
来源：http://hz.c1oappe.top/gtcrnistwp.html

PHP:  implode(",", $items);
来源：http://hz.quarkkingdee.top/gtcbehqbyj.html

JS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtyuefdncc.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtzdxgaiqm.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gtlauffjkv.html

Go:   strings.Join(items, ",")
来源：http://hz.0kj1m.cn/gtnrvprebc.html

Ruby: items.join(",")
来源：http://hz.yj202588.top/gtmvmpoyui.html

C#:   string.Join(",", items)
来源：http://hz.dashuyun.cn/gtxlceypeq.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtaltfeqas.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtyizgphxn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ybcxt.top/gtdgomrtcr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtzdwuwpzd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtqibzwoos.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.0kj1m.cn/gtpcifhwsi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cdnleiting.top/gtwicenhps.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.0kj1m.cn/gtaduiwnvx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daxiang520.top/gtslmeoyly.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnxiangtu.top/gtovikyrwu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xinyue.icu/gtoahpikvk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jqgfzy.top/gtnijuhxdn.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtjyiswvkw.html

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gttghovuna.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtdxyfeanb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gtwhubxrtg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtehigbaeq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtobojgqzk.html

[E11] 反转字符串
来源：http://hz.yvedp.cn/gtiflorjyx.html

Py:   s[::-1]
来源：http://hz.iojbl.cn/gtlmghmoea.html

PHP:  strrev($s);
来源：http://hz.jqgfzy.top/gthxwjjauu.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtnjraqlgn.html

TS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtkxnhjffd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fzhhl.top/gtufwjcufo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aizwys.cn/gtpbewyeuv.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gthtxxkmld.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtgsfxgeev.html

[E12] 统计某字符出现次数
来源：http://hz.jiagoushi.top/gtblllmdxr.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gtahixumfr.html

PHP:  substr_count($s, "a");
来源：http://hz.shanyushiyangtech.top/gtzfmcujah.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtgqcomtdk.html

TS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtumglvtnx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gtehzmmcnp.html

Go:   strings.Count(s, "a")
来源：http://hz.chenzaomai.com/gtmvllaxin.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtnszmotbt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sxryk.cn/gthfmyevto.html

[E13] 逐字符遍历
来源：http://hz.aizwys.cn/gtlwetqtgc.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtzafvbnkq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gtqeggadvv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtpxfaowsk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtfkgxkyop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gtcvxpdepu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj202588.top/gtyrazhkmo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yueranfly.top/gtiihlitkt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tianlin.xyz/gteiloumod.html

[E14] URL 编码与 Base64
来源：http://hz.xingfuxueyuan.xyz/gtjibbuofe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtupkebimv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gturflvewz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.52xcode.cn/gtipsweiks.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xziqi.cn/gtmrbxhnus.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ywan-chungtsiang.top/gtnxligiwt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtcrkddnqy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cdnleiting.top/gtkwehagvf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtnfjshilj.html

[E15] HTML 转义 / 反转义
来源：http://hz.shuidangran.top/gtxtuorflg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigfzy.top/gtqytwskun.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ywan-chungtsiang.top/gtropqqaws.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gtvirulrpo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xingfuxueyuan.xyz/gteqsxdvgf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cashguo.top/gthmuqrzpm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.smart0.xyz/gtpzvderkl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gzhubu.top/gtsvgadeys.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.bjfxy.top/gttxluyfox.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtzluwdbrq.html

Py:   f"{1234567:,}"
来源：http://hz.cdnleiting.top/gtydjgbwow.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtfwfjreqt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zdqjudy.top/gtednmeabv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtjfxxubtn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtgmzisljq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ivvv.top/gtqafksdch.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cheryme.top/gttyjebgxy.html

C#:   1234567.ToString("N0")
来源：http://hz.sweek.top/gtcoporaae.html

[E17] 首字母大写
来源：http://hz.yvedp.cn/gtjygiqnmb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtkqanitaj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dashuyun.cn/gtdhwfdbff.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtoamycgvr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtrwyrherp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.andypj.xyz/gtzsxnzujg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.c1oappe.top/gtiftcuxti.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtwixijjig.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtkkdaccnt.html

[E18] 模板占位符替换
来源：http://hz.ydjk.org.cn/gtlucuwbcq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtyzileyjq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxinkj.top/gtqzgydjtb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtjvukbtom.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtjllazlrf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nwbrower.top/gtgwzcpopc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtcuhfppuf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gtknhjgmfl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtxyeusdon.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gtfmznwemf.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtuvrrtgdg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtmnkwuvfs.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtbatqnyfo.html

TS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtgxhldxse.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtnwkyjied.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtczjiierp.html

Ruby: s.lines
来源：http://hz.tianlin.xyz/gtcuinsjoy.html

C#:   s.Split('\n')
来源：http://hz.sufxvd.cn/gtzdjcpaik.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangtech.top/gtmysymdmc.html

Py:   if not s:
来源：http://hz.tianlin.xyz/gtvpjtajje.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtibybohpw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.kuanghao11.cn/gtlzmcmjqv.html

TS:   if (s === "") {}
来源：http://hz.jinyuanbaomall.cn/gtzzodcxun.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gthnjnbicu.html

Go:   if s == "" {}
来源：http://hz.yongpay.top/gtdtkmtetp.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtubhofcmm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fengsongda.top/gtrdcmhrwg.html

[E21] 超长截断加省略号
来源：http://hz.gzhubu.top/gtwrobapco.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtctxvbyrb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtjeqvzijd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtghturdqa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtydlryxwr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtmjodyynf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtfbhbkykr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuetiantiany.cn/gttuhznynp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yonumen.top/gtekracgwc.html

[E22] 字节长度与字符长度
来源：http://hz.ywan-chungtsiang.top/gtgirkrvxb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtryjckecv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtdriwepqp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtctzakqdh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtahxrudlp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.pengpengdd.cyou/gtjnxaukgv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtiehksewx.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gtzdoaojpx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sxryk.cn/gtrjlolzrf.html

================================================================================
来源：http://hz.jianghu66.top/gtygymxnbo.html

F. 文件与目录
来源：http://hz.jinghuilouyu.cn/gtynbaxxfw.html

================================================================================
来源：http://hz.316326.xyz/gtuhvpvhkt.html

[F01] 读取整个文件
来源：http://hz.0kj1m.cn/gtfboakror.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxuanxn.top/gtclemycqc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhixingplan.top/gtsqaagbqs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtblvawqmt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xinyue.icu/gtqtuukgop.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtxgidciky.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xinyue.icu/gtzbpzfnog.html

Ruby: File.read("a.txt")
来源：http://hz.hysaishi.cn/gtmbbdwsbc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.vqdsnc.cn/gtiltvhqcm.html

[F02] 逐行读取文件
来源：http://hz.gaohongyu789.top/gtkhkilzfb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gtkqhnbbfs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtxcxxtkgq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtgrpvsgtf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtiywjczur.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtvsrxibtb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pycfn.com/gtxntrykwl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.316326.xyz/gthquxbjtb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtkiqxmrsl.html

[F03] 写入文件（覆盖）
来源：http://hz.birdmap.top/gtjjaxbldv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cdnleiting.top/gtszrgnicw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtjgqdoevl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtpsftcdvn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtwgdwexhu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtpuknlolg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hongshengwenyu.top/gtughkrghw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gtpcsmblod.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gttqlovsax.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangkeji.top/gtvmjxkwvk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aizwys.cn/gtgbprween.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fengsongda.top/gtuthrlcmq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtppkpdffi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtgudiawxx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aibaodan.cn/gtahcwobqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yongpay.top/gtlvnhlmde.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj202588.top/gtzhndbwpi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinghuilouyu.cn/gtkeztjvdj.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtjzdhpzaw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtwbhegotb.html

PHP:  file_exists("a.txt");
来源：http://hz.xinyue.icu/gtnbsvvhla.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtsixnaofl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtacplmngi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gttuoivfzm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangdashe.top/gtdymjzoyw.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhongyouzk.top/gtsmktbekt.html

C#:   File.Exists("a.txt")
来源：http://hz.jinghuilouyu.cn/gtmagwwtbm.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtsvwypsdy.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtpbpjcaml.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtcczyuhfl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtdksotagh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gttwsynfej.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gthyiqlfau.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gtrwihcqbq.html

Ruby: File.delete("a.txt")
来源：http://hz.daria6918.cn/gthhpitfqn.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gtczsdujtf.html

[F07] 创建目录（含多级）
来源：http://hz.shangyingyoupin.top/gtqmhkafik.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtmcpkxgeu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtfjguytuw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtkgbficqz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtpybaauzt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.bjfxy.top/gtfhfqqraa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtmcsfdnss.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtgynrogwa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guannengcc.top/gttjkktlev.html

[F08] 遍历目录
来源：http://hz.nwbrower.top/gtmikkxyff.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guowangkeji.top/gtkhakhjhc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gtszxdnlrn.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtquauzlvq.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtqmhxwmec.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtonwliitr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtxkgezeyl.html

Ruby: Dir.children("dir")
来源：http://hz.havefunace.top/gtwgifdbsf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.snrcjt.cn/gtytbureol.html

[F09] 获取文件大小
来源：http://hz.gzhubu.top/gtyofgqrnl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aibaodan.cn/gtjhqlxboe.html

PHP:  filesize("a.txt");
来源：http://hz.jinyuanbaomall.cn/gttsncalzu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtlptpogyi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtxkflyrxt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtvtkanlox.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinyuanbaomall.cn/gtbwtbaccu.html

Ruby: File.size("a.txt")
来源：http://hz.zhoulong.xyz/gtmsmuwjgu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gttsfjklga.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtxtpegvnc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtbrccpsty.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xylfe.cn/gthepbzpsx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtpiokzhhb.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gtsbzabolh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gtwzujqsss.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtmjisipsb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtusoetlus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtqcwoszpd.html

[F11] 复制与移动文件
来源：http://hz.pengpengdd.cyou/gtyxkavxln.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtpuysrgzw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtkuwrenov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gttdhvkyif.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtjhxobucb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.pengpengdd.cyou/gtpydxsguw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigfzy.top/gtzmxjlxhk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtlahrtast.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtdjpyiorj.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtcwfphbko.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtbbsztdbj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aizwys.cn/gtvvievkdv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtosvdibxh.html

TS:   // 同上
来源：http://hz.feifeiyinyue.top/gtbjiiyjgz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtqfxihjcn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zdqjudy.top/gtgyqnflro.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtaciqxbtn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jlsjyb.cn/gtnyightqm.html

================================================================================
来源：http://hz.cucudq.cn/gtsznfdfsq.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtxkttmahh.html

================================================================================
来源：http://hz.guannengcc.top/gtsbluknqz.html

[G01] 定义类
来源：http://hz.shanyushiyangkeji.top/gttryjbldu.html

Py:   class User: pass
来源：http://hz.shanyushiyangkeji.top/gtokbawmcp.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtgngsfnsv.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtmfxukhtk.html

TS:   class User { name: string = ""; }
来源：http://hz.gzhubu.top/gtmznaobzu.html

Java: class User {}
来源：http://hz.hammf.cn/gtrykrsxba.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtdjmdzogs.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtoottuzyn.html

C#:   class User {}
来源：http://hz.yj202588.top/gtdctmzrho.html

[G02] 构造函数
来源：http://hz.xziqi.cn/gtcrkudurx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jyoumei.cn/gtrbnkwluj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenjidiqi.icu/gtnecvximy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtsfcohrnt.html

TS:   constructor(public name: string) {}
来源：http://hz.jinghuilouyu.cn/gthggbnokj.html

Java: User(String name) { this.name = name; }
来源：http://hz.tian-w.cn/gtxeutxond.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangdashe.top/gtxahzjdas.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtijdmqvbu.html


<!-- 参考信息 -->