代发 wailian999

Go:   strings.Index(s, "x")
来源：http://hz.52xcode.cn/gteiqlhrdz.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gthwpiywkz.html

C#:   s.IndexOf("x")
来源：http://hz.yvedp.cn/gtquplprty.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtdkyxthbf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydzc1.top/gtgeowdmyt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenzaomai.com/gtcoomwtyp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuanzx.com/gtvazyfybq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shanyushiyangtech.top/gtckwyugek.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtalziyezi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ppjwa.cn/gtkhaccsfd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.kuanghao11.cn/gtosoojmqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sxryk.cn/gtnqdsdvqn.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtqzxmuyli.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.aibaodan.cn/gtekgzlswl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hongshengwenyu.top/gtsjkchdea.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtiumrleoz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtjatrwzry.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtxwsvghaq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hywenlv.cn/gtyhdqvhwz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.havefunace.top/gtrvjhirdn.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxuanxn.top/gtzxiyxvtr.html

[E07] 按分隔符拆分
来源：http://hz.tanke756.top/gtwexvzfbs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtnghyjkry.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gtiixcidjr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtwmlzbmhh.html

TS:   s.split(",")
来源：http://hz.zhixingplan.top/gtybgemfmu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtyicuemjb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.0kj1m.cn/gtefbnzlbf.html

Ruby: s.split(",");  s.split
来源：http://hz.zhijiandao.cn/gturedwzwf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cashguo.top/gtubmzuhvp.html

[E08] 数组按分隔符合并
来源：http://hz.gogol.net.cn/gtsbppywry.html

Py:   ",".join(items)
来源：http://hz.zdqjudy.top/gtasjmnszo.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtofalhuqg.html

JS:   items.join(",")
来源：http://hz.mhx1999.top/gtwhsbdjrq.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtvlrvgfmc.html

Java: String.join(",", items)
来源：http://hz.jinqigfzy.top/gtgkxbecsy.html

Go:   strings.Join(items, ",")
来源：http://hz.gotoacloud.top/gtpzibpxbk.html

Ruby: items.join(",")
来源：http://hz.xinyue.icu/gtueicufpx.html

C#:   string.Join(",", items)
来源：http://hz.redwolf501.top/gtowylhhqo.html

[E09] 去除所有空白字符
来源：http://hz.cdnleiting.top/gtlrkybmea.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guannengcc.top/gtcvjvtqgs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yonumen.top/gtovygsqzh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gtlzqxxbnf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtpzawpnsn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aibaodan.cn/gtqeavsasu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yongpay.top/gtyldfbzyl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sysykeji.top/gtkvupskpc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nwbrower.top/gtqtvtggnu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dashuyun.cn/gtdtmdzcen.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxinkj.top/gttvsvumhf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtwpvgxtfa.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtnpepouzj.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtjnxjfdmh.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtqeyrswrb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dashuyun.cn/gtdtmtxdmw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gttrarfytr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.svipenyu.cn/gtzgacqiuv.html

[E11] 反转字符串
来源：http://hz.yj20258888.top/gteemeuqoa.html

Py:   s[::-1]
来源：http://hz.redwolf501.top/gttzyffpkw.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gttmlufihw.html

JS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtwnnymuos.html

TS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtbqoyiqda.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yonumen.top/gtmlxfgcfa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gtbngoksko.html

Ruby: s.reverse
来源：http://hz.zhixingplan.top/gtdmaoqgis.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtdpkxwtpu.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtizujauwr.html

Py:   s.count("a")
来源：http://hz.ydzc1.top/gtaraberek.html

PHP:  substr_count($s, "a");
来源：http://hz.zycfv.cn/gtoqiuzlyh.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtgthucxrn.html

TS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtoxkalubq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hfpthk.cn/gtudhdnqmh.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gtczufefzt.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtewejobjk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtxaylxwnc.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtdidfhfte.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gttikbvqpq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xuanzx.com/gttbzqbjia.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtqefqaamu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hysaishi.cn/gtolskpibq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhijiandao.cn/gtgkjhsaft.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhoulong.xyz/gtehpmbzoe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shangyingyoupin.top/gtuvegxvcn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtpdsyhzaw.html

[E14] URL 编码与 Base64
来源：http://hz.gaohongyu789.top/gttehncgvw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtwtngijbx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gttxrbjjlu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhoulong.xyz/gtqlxsysfy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gtgmjujomh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daria6918.cn/gtdfdtuwjr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtbumdffir.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gtrydgydxm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtxazvmawd.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhiwuduotai.top/gtcbdorzqf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuanzhike.top/gtgfpkctvv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtdyxmynkw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hywenlv.cn/gtrqtyicos.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aizwys.cn/gtwdvttvra.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gtzadaqrjx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtircieowf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuetiantiany.cn/gttqkcnjfy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pengpengdd.cyou/gtqmtppuaj.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtwugpwmpx.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gttufqwdqt.html

PHP:  number_format(1234567);
来源：http://hz.jqgufenzy.top/gttmroxwkh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtkskpzyba.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtyjhqamaj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtwbattagg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtiinhtxtk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daria6918.cn/gttrrdotxe.html

C#:   1234567.ToString("N0")
来源：http://hz.ybcxt.top/gtsjvpjhvi.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtnmebujmp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtpzecjeui.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtivsvggaj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.0kj1m.cn/gtrruagexx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtufeggotz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daria6918.cn/gtqktpzphp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtnsoeanpj.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gtdgpjfshs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cheryme.top/gtliwdfzpc.html

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gttsofqlzi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gtokgcwdao.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtvntlawck.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangshuangyany.cn/gtpukxiwdf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ivvv.top/gtsdlfkvaz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jlsjyb.cn/gtvsjdpxen.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtaopuralw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuanzx.com/gtphofxiol.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shangyingyoupin.top/gtptffubiz.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtftjavfyt.html

Py:   s.splitlines()
来源：http://hz.yongpay.top/gtlzemdqty.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigufen.top/gtdpxcdvzh.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtxbfzpfsg.html

TS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtaeauwtog.html

Java: s.lines().toList()
来源：http://hz.xuetiantiany.cn/gtwcqmfrva.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtvpdrmetd.html

Ruby: s.lines
来源：http://hz.guowangkeji.top/gtcxteysyb.html

C#:   s.Split('\n')
来源：http://hz.yj20258888.top/gtxqfyozjb.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtvlzqkcbi.html

Py:   if not s:
来源：http://hz.yvedp.cn/gtjbzlpjoy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.0kj1m.cn/gtdsjpymox.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yueranfly.top/gtikjbgvlf.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gtcynpekmb.html

Java: if (s.isEmpty()) {}
来源：http://hz.yvedp.cn/gtqbnwapqx.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtozyalsbs.html

Ruby: if s.empty?
来源：http://hz.feifeiyinyue.top/gtzenjmstb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gttwrbvked.html

[E21] 超长截断加省略号
来源：http://hz.hysaishi.cn/gtqjvqkvvd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aizwys.cn/gtghbnaupr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.birdmap.top/gtskqlwmdw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtemrqkfgl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtudcqqftk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtdsgytujg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtecjpzgqw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.meibo888.top/gtqhcgnrwk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtpbelxphj.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtiyeaarzt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydzc1.top/gtmxnrmqhi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtwgpxccye.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtifgfwcxr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gtwyzjrats.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtitwrgmaj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tanke756.top/gtwibpvxec.html

Ruby: s.bytesize;  s.length
来源：http://hz.vqdsnc.cn/gtxvqzgmgv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtgwwthxoe.html

================================================================================
来源：http://hz.iojbl.cn/gtyhdvrsdp.html

F. 文件与目录
来源：http://hz.shangyingyoupin.top/gtdcjzoikq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtboyngxll.html

[F01] 读取整个文件
来源：http://hz.xinyue.icu/gtwbowuhtg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtlsspuwfv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtebzsfbry.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gtnvjilsfx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sysykeji.top/gtwrpnugjz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtiojajpur.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dianchejie.cn/gtpqwdgppk.html

Ruby: File.read("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtkfimndmf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenlongwang.top/gtcpecxklp.html

[F02] 逐行读取文件
来源：http://hz.nanxinkj.top/gtdynyasby.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydzc1.top/gtgdknxbxz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hywenlv.cn/gtgqhhaynz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtgpilqpol.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtbijmfxyr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtymkazaqo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuxming.cn/gtmvlijshi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nanxuanxn.top/gtredopxtv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtadbbuaci.html

[F03] 写入文件（覆盖）
来源：http://hz.chenlongwang.top/gtelwrvuhd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtxhbzkvvf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtzgawuxca.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gteaxbltrt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtjlkgrdth.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gttrtpxskx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.316326.xyz/gticvutzkq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hammf.cn/gtkkkyzwiq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.svipenyu.cn/gteemhzetc.html

[F04] 追加写入文件
来源：http://hz.ywan-chungtsiang.top/gtynbxheiu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gtovrgajys.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtzrlshnzc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtflqioyij.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtccetcayk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtvyhieqpg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daxiang520.top/gtpaildovg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gtctzrwovv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.haohaochexian.top/gtqkebuopd.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtybmbdfmo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtzednrijn.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtooochkzv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtrrestwoa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtdrrcflqf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtilzqqdpr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigfzy.top/gtbjzjyoxy.html

Ruby: File.exist?("a.txt")
来源：http://hz.sweek.top/gtxtufawep.html

C#:   File.Exists("a.txt")
来源：http://hz.chenjidiqi.icu/gtrcyafkux.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtbmgobcui.html

Py:   os.remove("a.txt")
来源：http://hz.zdqjudy.top/gtzvnloajx.html

PHP:  unlink("a.txt");
来源：http://hz.chenlongwang.top/gtoedirjnm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtbgnhzhqh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtwpatsvzg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gthzpaqnob.html

Go:   os.Remove("a.txt")
来源：http://hz.c1oappe.top/gtixjcduxq.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gtkbaimzfb.html

C#:   File.Delete("a.txt");
来源：http://hz.fzhhl.top/gtgtmevyfg.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtfllbjzjn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtandobxxq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtknitryzm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtpkgtudwz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtbxqgxsob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cashguo.top/gtbpqnvhuc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.snrcjt.cn/gtcelqyseo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtxgdkyeck.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sysykeji.top/gtzqimkcvn.html

[F08] 遍历目录
来源：http://hz.yanxiufei.cn/gtbfxclryi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtviojfykq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.52xcode.cn/gtrrtnsabg.html

JS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtqnnjikqn.html

TS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtdbwyvael.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gteewpbzej.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pengpengdd.cyou/gtgxkapvws.html

Ruby: Dir.children("dir")
来源：http://hz.ybcxt.top/gtqexnimyk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pycfn.com/gtpaqewxuh.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtutskfopl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sysykeji.top/gteahqmpkt.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtadsxpdpd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtwwmqccoc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtpaoqvptd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtlafolclv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gttfhrttuz.html

Ruby: File.size("a.txt")
来源：http://hz.kuanghao11.cn/gtrjlqorgw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtugnwnboz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtpxoekrhp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtqfbjbjwb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtnyulajen.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtyowvuspc.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gteesryrxh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenjidiqi.icu/gtedgpzpwt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtvdnmbeki.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtucyintgj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigufen.top/gttwfnjnbr.html

[F11] 复制与移动文件
来源：http://hz.cqqwz.cn/gtiamnatlt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtitjokhti.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuanzx.com/gtwglowrob.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtwfqhisrh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtixtjzioe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guowangkeji.top/gtxsapajfs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.bjfxy.top/gtciotohmb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtdfbgcmij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jyoumei.cn/gtdtqmcwya.html

[F12] CSV 读写
来源：http://hz.cheryme.top/gtmkkyzpko.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yongpay.top/gtgykkxdyv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yangfankeji.com/gtgsduqsnq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.svipenyu.cn/gtmzmvkgkg.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtwermznza.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtvpyjrnzs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj202588.top/gteszidlgd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gthecxvyab.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gteltqxxla.html

================================================================================
来源：http://hz.hammf.cn/gtlqbwmguv.html

G. 面向对象
来源：http://hz.9152youxi.cn/gtdwgqzphw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxxvywyin.html

[G01] 定义类
来源：http://hz.daxiang520.top/gtnlxvbqat.html

Py:   class User: pass
来源：http://hz.0kj1m.cn/gtcwnqmuxf.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtrnftpyxz.html

JS:   class User {}
来源：http://hz.snrcjt.cn/gtdnhkquyl.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtykstblut.html

Java: class User {}
来源：http://hz.shzxlz.cn/gtwdzqpahr.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtekhjudnz.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtabfpiles.html

C#:   class User {}
来源：http://hz.jinghuilouyu.cn/gtumwrukkm.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtbvevvpbw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shuidangran.top/gtlevxomvh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtytiajjwi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtexphknca.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gtozkddywn.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtclwpterj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gzhubu.top/gtondwxeaj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtndskgvyt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtmoajwtqp.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtywevssga.html

Py:   self.name = "x"
来源：http://hz.zhixingplan.top/gtuvbhgabr.html

PHP:  public string $name = "x";
来源：http://hz.hywenlv.cn/gtwrpfyhiu.html


<!-- 参考信息 -->