代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gaohongyu789.top/gtybauqqbl.html

[E03] 截取子串
来源：http://hz.vqdsnc.cn/gtvuxppfzi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenlongwang.top/gtxqbbelwh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.0kj1m.cn/gtsruzxgwr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtljnkrblf.html

TS:   s.slice(1, 4)
来源：http://hz.wangdashe.top/gtvwfmmdrm.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtsxxayhwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtlffztlen.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jianghu66.top/gtvtqmjrjs.html

C#:   s.Substring(1, 3)
来源：http://hz.cqqwz.cn/gtssivtnrt.html

[E04] 查找子串位置
来源：http://hz.ybcxt.top/gtupwzjiul.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhiwuduotai.top/gtwyophjlx.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gteabloyoj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnqzz.top/gtnydjymrp.html

TS:   s.indexOf("x")
来源：http://hz.ppjwa.cn/gtwkajhixk.html

Java: s.indexOf("x")
来源：http://hz.redwolf501.top/gthdetsipy.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gtupgqwrxr.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gthfelhcmo.html

C#:   s.IndexOf("x")
来源：http://hz.wangdashe.top/gtrpdkgjgn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xinyue.icu/gtecmyyupo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yonumen.top/gtcsdbzzxe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ivvv.top/gtfhkhszhr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gtictndxnu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hywenlv.cn/gtyunbghhc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtcdfszxpa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.wangdashe.top/gtbohvpuzs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yvedp.cn/gtqlhhfjyg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigfzy.top/gtsigxwxkt.html

[E06] 替换子串
来源：http://hz.meibo888.top/gtcksvxmlh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenlongwang.top/gtvjyxashg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jiagoushi.top/gtnxepowuw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtvdxjkaxf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtygydontv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtcdiaxqum.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigufen.top/gtavszbbbq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.9152youxi.cn/gthydkzmnb.html

C#:   s.Replace("a", "b")
来源：http://hz.snrcjt.cn/gteimslmyx.html

[E07] 按分隔符拆分
来源：http://hz.hnxiangtu.top/gtuxqhebzw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hongshengwenyu.top/gtymagdedl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ydjk.org.cn/gtyowyucoq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinyuanbaomall.cn/gtcsgrnfve.html

TS:   s.split(",")
来源：http://hz.guannengcc.top/gttffyotxn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.birdmap.top/gtzldfcepo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtaylvdazg.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtljvknqyc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gtwlhfgamp.html

[E08] 数组按分隔符合并
来源：http://hz.pengpengdd.cyou/gtxxztgkpq.html

Py:   ",".join(items)
来源：http://hz.nanxuanxn.top/gtxqgxkabm.html

PHP:  implode(",", $items);
来源：http://hz.aizwys.cn/gtaspkpoap.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gtqzvzogqq.html

TS:   items.join(",")
来源：http://hz.ivvv.top/gtplccnwdk.html

Java: String.join(",", items)
来源：http://hz.dianchejie.cn/gtxhuhgobo.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigufen.top/gtabdvbjwb.html

Ruby: items.join(",")
来源：http://hz.yuanzhike.top/gtcgnvkrou.html

C#:   string.Join(",", items)
来源：http://hz.fengsongda.top/gtbuqbubvr.html

[E09] 去除所有空白字符
来源：http://hz.cashguo.top/gtbdsdjzko.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtabxlgvtn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gtmgmtcwet.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtjkdvdtdk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtkzxeirpz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shzxlz.cn/gtocixoqnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gthoqtfvds.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtlqsnmwum.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daxiang520.top/gtoxamnapx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gthimqopqf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jiagoushi.top/gtaxxungoy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xuetiantiany.cn/gthtyjnzyv.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtbgzpzflz.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtjbgslgzr.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtitxzywtn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.bjfxy.top/gtihvvdioc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xinyue.icu/gttodyzbcu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigufen.top/gtqyptovze.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtndjzaqev.html

Py:   s[::-1]
来源：http://hz.yuxming.cn/gtsrbdjzgg.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtnwbofuhr.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtlxrqmulk.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtldurziog.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ehwqpu.com/gthkrcnipo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhijiandao.cn/gtgmzguqrb.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtlzmyjtol.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gthsxgfgss.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangkeji.top/gtdubqqmqr.html

Py:   s.count("a")
来源：http://hz.jyoumei.cn/gtdxpinuzv.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtyhbrcshn.html

JS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtmrccqnzm.html

TS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gtoikehyci.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuanzx.com/gtxytlvjfg.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtwmhcczug.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gthbrijlwd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gogol.net.cn/gtbkgwngdv.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtmrlookly.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtfmzvdubx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhixingplan.top/gtshxvwmqp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gtevyxpawz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtmygwpyzu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.kuanghao11.cn/gtgvknkzqa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtokmwleek.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhoulong.xyz/gtqocurdeq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtlgfpsjrx.html

[E14] URL 编码与 Base64
来源：http://hz.zdqjudy.top/gtsapziqws.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gthlacaqqu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gtatylutfy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tanke756.top/gtqvdwuera.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258888.top/gtjcnmtskr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydzc1.top/gtybdntssx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dianchejie.cn/gtkhvwyyoc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtflniprtc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.feifeiyinyue.top/gtsnpybbkl.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtfqncgfie.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cucudq.cn/gtbawskxvp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sweek.top/gtgypemucf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jianghu66.top/gtidmjzfkd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yueranfly.top/gtbzslyyqd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.pycfn.com/gtzbzuouxq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtxdsqcdjs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtznzlbzlq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cdnleiting.top/gtrmzaihvt.html

[E16] 数字千分位
来源：http://hz.jianghu66.top/gtuufyznis.html

Py:   f"{1234567:,}"
来源：http://hz.tianlin.xyz/gtsswlewwa.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangkeji.top/gtmdwtpzpw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtnsowamcx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtujekexcp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydzc1.top/gtjyrnyipv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuetiantiany.cn/gtemurmcda.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shuidangran.top/gtvekyxzzu.html

C#:   1234567.ToString("N0")
来源：http://hz.ydzc1.top/gtfakfzqag.html

[E17] 首字母大写
来源：http://hz.kuanghao11.cn/gtuobhlutc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.andypj.xyz/gtkntvqzmv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuanzx.com/gtsmelekzu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aizwys.cn/gtxzehogcd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtkotuwdgo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtletrxfwp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtvjrhxwjt.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gtklwfsniq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.haohaochexian.top/gtlccvbqzm.html

[E18] 模板占位符替换
来源：http://hz.52xcode.cn/gtkzkjuldo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtqyryubhp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.pengpengdd.cyou/gtjsjndqvb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtlseexehv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtuycfbhis.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sxryk.cn/gtfpmyifxr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yuxming.cn/gtmbeezita.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.snrcjt.cn/gtpajchsmh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jlsjyb.cn/gtknbkjxcb.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtpjpnyent.html

Py:   s.splitlines()
来源：http://hz.hysaishi.cn/gtnguuelpp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tanke756.top/gtfgztbtvn.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtdcrqferg.html

TS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtijvafppg.html

Java: s.lines().toList()
来源：http://hz.mhx1999.top/gtozpxcrgx.html

Go:   strings.Split(s, "\n")
来源：http://hz.aizwys.cn/gtldkrfnvy.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtzrruajrv.html

C#:   s.Split('\n')
来源：http://hz.gogol.net.cn/gtjnpfvzad.html

[E20] 判断字符串是否为空
来源：http://hz.nwbrower.top/gtzkrioskl.html

Py:   if not s:
来源：http://hz.hnqzz.top/gtmygadjbp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.mhx1999.top/gtghnbpnon.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jiagoushi.top/gtjuibxqfm.html

TS:   if (s === "") {}
来源：http://hz.birdmap.top/gtelwwhcto.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtsifzpkmv.html

Go:   if s == "" {}
来源：http://hz.pycfn.com/gtynvyainx.html

Ruby: if s.empty?
来源：http://hz.meibo888.top/gtqavlphot.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtqqrymayv.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtytkiygzh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.redwolf501.top/gtmpflxrlh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuanzhike.top/gtoqebgfji.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtmdyphfjo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtooimwpjt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtaegemrsa.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yangfankeji.com/gtdaeghcue.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhixingplan.top/gtccjusslc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtycggxjim.html

[E22] 字节长度与字符长度
来源：http://hz.shzxlz.cn/gtrmyxsizb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenlongwang.top/gtcwpunzuq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtvsujxwri.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtohkjmeyu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtowuscqor.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtnbgqwphv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtdmgizjgn.html

Ruby: s.bytesize;  s.length
来源：http://hz.svipenyu.cn/gtffgakcwy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtxxvnbcll.html

================================================================================
来源：http://hz.yuanzhike.top/gtqhtvaayv.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtmaxnyxxn.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtalixcywg.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gthbspthqg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.svipenyu.cn/gtpyplddud.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtukbmgltz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tanke756.top/gtvvituvia.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shzxlz.cn/gtnuvocpbk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtzmggngbf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gtksharafh.html

Ruby: File.read("a.txt")
来源：http://hz.jyoumei.cn/gtsrogemob.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gtkcyimjqs.html

[F02] 逐行读取文件
来源：http://hz.tanke756.top/gtuyxepera.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenzaomai.com/gtmqxzfstb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtfypwkwfe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtxktjdhvg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtovtbvump.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtguxkqzbr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.haohaochexian.top/gtnkaitxfb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtdzzrdqpz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gogol.net.cn/gtghuavqpo.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtgbqizzym.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtyjifbxde.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtpczclcjv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtnetqvunz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtrvegztqu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xziqi.cn/gtwvyqgetg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtvuuzweeq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigufen.top/gtmshbedjp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtnkjleije.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gtpdgfinsl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sweek.top/gtuvumqvrk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuanzx.com/gtjkwavtqa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtqakgldwo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtuqgfvjzx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtrddcmyry.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinyuanbaomall.cn/gtybkczkzq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jyoumei.cn/gtsmjocaly.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtllulrqgi.html

[F05] 判断文件或目录是否存在
来源：http://hz.vqdsnc.cn/gtgvbqhrhu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtxsalkulg.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtpiuhkkht.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtuyscqfpz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtrakkcgjr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtmgpvpvhc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtbqirxbht.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtywgqxdvj.html

C#:   File.Exists("a.txt")
来源：http://hz.zhoulong.xyz/gtvalbsjbx.html

[F06] 删除文件
来源：http://hz.pycfn.com/gturkipcyi.html

Py:   os.remove("a.txt")
来源：http://hz.zhongyouzk.top/gtxpshrkrc.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtpjsgngzz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtlnwmgjmc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtmskqnanz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtbtdmfcko.html

Go:   os.Remove("a.txt")
来源：http://hz.hfpthk.cn/gtuhakptes.html

Ruby: File.delete("a.txt")
来源：http://hz.tanke756.top/gtxxtwbfls.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtcjgprnhb.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gtydmaqxcn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gthegejtrm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sweek.top/gtwdxkdxdr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtemqbfzon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtpjsuizwg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtnrckgxfw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pycfn.com/gtmjtxvcvv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sxryk.cn/gthpvnvffg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gtexjfupsk.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gtqzmxsdsy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sweek.top/gttzyorvcn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sufxvd.cn/gtmiyuovha.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtthrfelyk.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangshuangyany.cn/gtdeijikdv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtggzfnruc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gtwqlefznq.html

Ruby: Dir.children("dir")
来源：http://hz.aibaodan.cn/gttpxcbqhv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgufenzy.top/gtsmgwwlae.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gthqjzyafm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hysaishi.cn/gtsceyidyc.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtvnzrqjik.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtazotzxlw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtjvvxrslo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gthccgogma.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtqgepukqz.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtxzrazxtb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtimfpukzs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gttrvgpwwo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtkygdikdk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sweek.top/gtilkpqpbv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtyfxhazgr.html

TS:   path.extname("a.txt")
来源：http://hz.meibo888.top/gtivktwamt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zycfv.cn/gtjntcjotc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtpjlcrovm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtltazkfka.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hywenlv.cn/gtfeaeqfrn.html

[F11] 复制与移动文件
来源：http://hz.chenjidiqi.icu/gtskmmgwdn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtarbainjw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jlsjyb.cn/gtxxxcsxmg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtiscxshdh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtpmumsuhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.vqdsnc.cn/gthxviriod.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangshuangyany.cn/gttjsxqjbr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtbiseuqnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhongyouzk.top/gtbebyyodq.html

[F12] CSV 读写
来源：http://hz.pengpengdd.cyou/gtduibaijc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.svipenyu.cn/gttewqfwcq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtxhzrfcbu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zycfv.cn/gtqernkyol.html

TS:   // 同上
来源：http://hz.xziqi.cn/gtinrvxqvl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtvlbxkllv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.smart0.xyz/gtyobfvnmo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtdshvaqpn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtdagxkibw.html

================================================================================
来源：http://hz.chenlongwang.top/gtqvwvdvcn.html

G. 面向对象
来源：http://hz.meibo888.top/gthyixfqfd.html

================================================================================
来源：http://hz.yonumen.top/gtmwvwekas.html

[G01] 定义类
来源：http://hz.cucudq.cn/gtqikfbgav.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtrrzlnump.html

PHP:  class User {}
来源：http://hz.yangfankeji.com/gtwrlnhrds.html

JS:   class User {}
来源：http://hz.0kj1m.cn/gtllqkyzwh.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtqrvebfuo.html


<!-- 参考信息 -->