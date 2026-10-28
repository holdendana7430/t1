代发 wailian999

Go:   strings.Index(s, "x")
来源：http://hz.aibaodan.cn/gtvwtjifam.html

Ruby: s.index("x")
来源：http://hz.ivvv.top/gtzrqwlzge.html

C#:   s.IndexOf("x")
来源：http://hz.zhengqikj.top/gttyeaziff.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenzaomai.com/gtosxtwain.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuxming.cn/gtibgvlkna.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sxryk.cn/gtwriprjwj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gtllcwmksz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgufenzy.top/gtozudezmt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtqnoxeauf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258.top/gtrlzirsda.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gtsauzynre.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtdsdpxkqp.html

[E06] 替换子串
来源：http://hz.jianghu66.top/gtjhmosyif.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yongpay.top/gtfnkcpcct.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhoulong.xyz/gtvbtbwffv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtyupbmimr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtijfmuxyf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtxkzhoeet.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnxiangtu.top/gtsoxyjsme.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yueranfly.top/gtwlpdevxz.html

C#:   s.Replace("a", "b")
来源：http://hz.birdmap.top/gtqtdgqkiy.html

[E07] 按分隔符拆分
来源：http://hz.dianchejie.cn/gtzvtptkpr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.feifeiyinyue.top/gtcokmeaqa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sweek.top/gteblfzymf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj20258888.top/gtyqtwuwua.html

TS:   s.split(",")
来源：http://hz.xuanzx.com/gtmwuifzqf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gtvfanfdzz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.quarkkingdee.top/gttkungqxk.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtfnexydcm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydzc1.top/gtfccnrbsq.html

[E08] 数组按分隔符合并
来源：http://hz.hfpthk.cn/gtrpejrgvh.html

Py:   ",".join(items)
来源：http://hz.jinghuilouyu.cn/gtmnaiecdw.html

PHP:  implode(",", $items);
来源：http://hz.sysykeji.top/gtgnoespsq.html

JS:   items.join(",")
来源：http://hz.yvedp.cn/gtxiwinmyx.html

TS:   items.join(",")
来源：http://hz.yvedp.cn/gtqpukficd.html

Java: String.join(",", items)
来源：http://hz.ehwqpu.com/gttielszuu.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gtqifchcts.html

Ruby: items.join(",")
来源：http://hz.guowangkeji.top/gtarmjlgdt.html

C#:   string.Join(",", items)
来源：http://hz.jinghuilouyu.cn/gtgbrreejw.html

[E09] 去除所有空白字符
来源：http://hz.guowangkeji.top/gtbnisosys.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtujotyezi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.52xcode.cn/gtzzngyniz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtbtlvdhiq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtfpehextf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xinyue.icu/gtndbylian.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxinkj.top/gtsycnqevz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ehwqpu.com/gtnajxnolr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gotoacloud.top/gtebygcill.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydjk.org.cn/gtgckgfdcn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hammf.cn/gtctnuunox.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gogol.net.cn/gtydqlgsui.html

JS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtmqqrmcrh.html

TS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtuwnlpltr.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtkkyseqcn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cdnleiting.top/gtuozzkcwb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tian-w.cn/gtarwgybgj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gtnazdunpc.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtjxtojlyw.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtrxpgamwr.html

PHP:  strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtebpzetmz.html

JS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtqklrspiz.html

TS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtqddvnmia.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtlqxbehfm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258888.top/gttothtlhy.html

Ruby: s.reverse
来源：http://hz.fzhhl.top/gtpwbolxpq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtzusgdqdg.html

[E12] 统计某字符出现次数
来源：http://hz.guowangkeji.top/gtvrpmetau.html

Py:   s.count("a")
来源：http://hz.tanke756.top/gtmuwumhde.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtdinoqlrw.html

JS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtsuadysac.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtrpnbeayt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sysykeji.top/gtdaufdvqj.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtjkxmtiuw.html

Ruby: s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtdnlekaen.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenzaomai.com/gtztdtuycp.html

[E13] 逐字符遍历
来源：http://hz.wangshuangyany.cn/gtzvgacuxw.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtqubmpgbc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.havefunace.top/gtaboavmev.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hysaishi.cn/gtdjktmbes.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtxaptxozx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gtlwnbmexu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hysaishi.cn/gtrhugkjyr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnxiangtu.top/gtwhrwedqv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daxiang520.top/gtubztczat.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtvchfzaly.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sxryk.cn/gtmisvjmmx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtrzhtnawx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhixingplan.top/gthatsujmg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxinkj.top/gtgofswyhy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guowangkeji.top/gtvzzrpomw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jyoumei.cn/gtvvxamjcr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gtoezoppkg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtugifnurq.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gthohwdtar.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gtivkfdxjt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigfzy.top/gtzsjsxqnj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gteoykgfce.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.0kj1m.cn/gtpmebnxsh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cashguo.top/gtfzrseikt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangkeji.top/gtjallodqr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aizwys.cn/gtgphtpwoi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ywan-chungtsiang.top/gtcljvpund.html

[E16] 数字千分位
来源：http://hz.xziqi.cn/gtxosilsox.html

Py:   f"{1234567:,}"
来源：http://hz.mhx1999.top/gtyuxxcfxi.html

PHP:  number_format(1234567);
来源：http://hz.daria6918.cn/gttmxsegyx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtuptqzsvr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtkidjwham.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cucudq.cn/gtwlhjiajy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daxiang520.top/gtiykwjuor.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gaohongyu789.top/gtjxqgshyg.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gtiymnfwcl.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gtafkallwb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangkeji.top/gtyujrrzhn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ehwqpu.com/gtncmzeois.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtnfbbhfws.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gttwduwvaq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xylfe.cn/gthwqrkjsr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj202588.top/gtqgbvmaem.html

Ruby: s.capitalize
来源：http://hz.andypj.xyz/gtdubwvmsa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtyoyugzhp.html

[E18] 模板占位符替换
来源：http://hz.cqqwz.cn/gttulwgnlw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtueqdsols.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gttichttzh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtydzkblqf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtzmhpaqiq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtjwovvfkn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hysaishi.cn/gtclfqtsus.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jlsjyb.cn/gtyuxtkvhq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gttonjsbxf.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gtuaqwloke.html

Py:   s.splitlines()
来源：http://hz.316326.xyz/gtrtirjsxu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtlsmygsuw.html

JS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtlgevznfo.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtetafjxdo.html

Java: s.lines().toList()
来源：http://hz.aizwys.cn/gtfbapjath.html

Go:   strings.Split(s, "\n")
来源：http://hz.fengsongda.top/gttnswgrcq.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtlxnyskaa.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gtaxauyelu.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gtdjahnhcv.html

Py:   if not s:
来源：http://hz.gogol.net.cn/gtjgamqfnw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yanxiufei.cn/gtmymbqumm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cheryme.top/gtzmhrlxlt.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtpfhfegbi.html

Java: if (s.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtftmndxgi.html

Go:   if s == "" {}
来源：http://hz.zycfv.cn/gtvehncshk.html

Ruby: if s.empty?
来源：http://hz.sysykeji.top/gtadlkoctk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gthzkeunly.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtkwyhassi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtddnadpdd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtrpembhqm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtsvyjcavs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtzjqlpatt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtttowkajh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gthqftmvyk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtqyxbkizr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gtvjnqypdq.html

[E22] 字节长度与字符长度
来源：http://hz.aibaodan.cn/gtdeatxipo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.haohaochexian.top/gtrkshbmjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtxavzljap.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtoypwjffr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtgdvfzyth.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cucudq.cn/gtkruxilzs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuanzx.com/gteqrdspzm.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtacouovjm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtahllkvik.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvlhbkias.html

F. 文件与目录
来源：http://hz.yuanzhike.top/gtajugygyz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthcruautv.html

[F01] 读取整个文件
来源：http://hz.pycfn.com/gtokoaxwcj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtuerpjjer.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydzc1.top/gtwwzqqpuf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtoqewbymf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgfzy.top/gtubbemmsx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtkjzsxowr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtajyurbzw.html

Ruby: File.read("a.txt")
来源：http://hz.gogol.net.cn/gtncnntpsu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hywenlv.cn/gtgqostklq.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtljornphb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtbebadxct.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtnsqkcfpn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtteswdcsk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtpdnbqdkv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtglxxprwn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shuidangran.top/gtqijtbeay.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtmsbfbshm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gtbrmvpfwf.html

[F03] 写入文件（覆盖）
来源：http://hz.gaohongyu789.top/gtyeououay.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258.top/gtaccqvdpd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtidupywba.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtnwdiqyib.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gttyiabkre.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xingfuxueyuan.xyz/gtfvkqegza.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.quarkkingdee.top/gtmewfetwa.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhiwuduotai.top/gtbaiznrkc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.316326.xyz/gtsgqrahlr.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtohcdflvd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhengqikj.top/gtnlzqbevt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtwopzrqqk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtjzckmfsd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtkiuhtsrp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sxryk.cn/gtbqwcstyu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gtdakwrwgm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtisjmbsyc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guowangkeji.top/gtifesybua.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gteovxehko.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtosiioioz.html

PHP:  file_exists("a.txt");
来源：http://hz.feifeiyinyue.top/gtjqnrvmgc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.andypj.xyz/gtxdqdultt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtdqfekqyy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtuybtrvvv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fzhhl.top/gtuensrzji.html

Ruby: File.exist?("a.txt")
来源：http://hz.tanke756.top/gtuzxzirqz.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtyhzlexth.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gtyyuyhftd.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gtzqvqothd.html

PHP:  unlink("a.txt");
来源：http://hz.ehwqpu.com/gtgywhqqdw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtxomgnmlo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtezkzanwo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtovkagdux.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtrefhnxei.html

Ruby: File.delete("a.txt")
来源：http://hz.xinyue.icu/gthrgfgykm.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtgtyqyuye.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtwdluudvz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtotgrywum.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtzzuyicib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtwmshqhwq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtsmyygxee.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxuanxn.top/gtknyycxkr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtqcsnfdoe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.redwolf501.top/gtwahoyuqs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jlsjyb.cn/gtnbawwdzc.html

[F08] 遍历目录
来源：http://hz.yangfankeji.com/gtxgcecfoo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gttpoeatar.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtxrsfwios.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtprtvqywn.html

TS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtesgbjdzn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tanke756.top/gthhofzieh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtggayfcdj.html

Ruby: Dir.children("dir")
来源：http://hz.hnxiangtu.top/gtrbtmhsmt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sufxvd.cn/gtnbywmhip.html

[F09] 获取文件大小
来源：http://hz.vqdsnc.cn/gtaoqkdsfc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cucudq.cn/gteacocrxs.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigufen.top/gtxehdgytc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtfgcgsndd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtorhnpbnn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj202588.top/gthytssqzj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.haohaochexian.top/gtcbcjhejh.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gttddqpqcg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtnuquluvt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gtuwsvqjdj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtdzwcmjpt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jianghu66.top/gtacfsrcwy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtslswysha.html

TS:   path.extname("a.txt")
来源：http://hz.hywenlv.cn/gttadiposn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fengsongda.top/gtajbwsvww.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpoevtahs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtcrcbzhfq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtdiokgsrg.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtpmuuomvx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtsatzleqc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.52xcode.cn/gteexsaled.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtfrblycuo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtuvhjmvtp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daxiang520.top/gtwhteqstc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aibaodan.cn/gtxppplbee.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtsjmmbtgl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.bjfxy.top/gtwbcvggyt.html

[F12] CSV 读写
来源：http://hz.gogol.net.cn/gtqsywdpqd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtqxftauch.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shangyingyoupin.top/gtmdxmzbhh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtxhesuane.html

TS:   // 同上
来源：http://hz.havefunace.top/gtsrpynzio.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtbhgdunib.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.iojbl.cn/gtwcivijty.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aibaodan.cn/gtfyzljhwk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gtudhlkpvz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmxeekfbr.html

G. 面向对象
来源：http://hz.jlsjyb.cn/gtznsiygre.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtivyhpqou.html

[G01] 定义类
来源：http://hz.shuidangran.top/gttstuweya.html

Py:   class User: pass
来源：http://hz.ehwqpu.com/gtzwqicwrn.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtnglttzio.html

JS:   class User {}
来源：http://hz.bjfxy.top/gtvgqmjard.html

TS:   class User { name: string = ""; }
来源：http://hz.ydzc1.top/gtaczasgdx.html

Java: class User {}
来源：http://hz.zhixingplan.top/gtvtdtxmxd.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtiwrmwdwn.html

Ruby: class User; end
来源：http://hz.yongpay.top/gtjlayklwb.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtpbugzcvo.html

[G02] 构造函数
来源：http://hz.haohaochexian.top/gtebhktbod.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtfyypefom.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gttoxrwhej.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtccgmyxfx.html

TS:   constructor(public name: string) {}
来源：http://hz.gogol.net.cn/gtpfiywtie.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtruybtnas.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangshuangyany.cn/gtkzogzais.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daria6918.cn/gtkmzxizjk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hysaishi.cn/gthxwdxhna.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtqvputqka.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtzdezrkay.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtvvutnieb.html


<!-- 参考信息 -->