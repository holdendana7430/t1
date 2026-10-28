代发 wailian999

TS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtbbfflhgh.html

Java: "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtgqdcuqyy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xziqi.cn/gthffkdbwz.html

Ruby: "ab" * 3
来源：http://hz.tian-w.cn/gtmhcefgmr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnxiangtu.top/gtkcdhzbct.html

[E03] 截取子串
来源：http://hz.meibo888.top/gtgphxzorj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.52xcode.cn/gtcdmxsnbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yonumen.top/gtopbvkxvj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yonumen.top/gtdyjoinle.html

TS:   s.slice(1, 4)
来源：http://hz.cucudq.cn/gtvocmgqpq.html

Java: s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtuammjoex.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhixingplan.top/gtjuepzhsq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nwbrower.top/gtpunovqcy.html

C#:   s.Substring(1, 3)
来源：http://hz.xuetiantiany.cn/gtaryiyijf.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gtrvfweklc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtlnmngnib.html

PHP:  strpos($s, "x");
来源：http://hz.zhaomingkeji.xyz/gtcjoukndv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shuidangran.top/gtdyoaiyqy.html

TS:   s.indexOf("x")
来源：http://hz.havefunace.top/gtrfampxrc.html

Java: s.indexOf("x")
来源：http://hz.zhixingplan.top/gtlutoxfpl.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gtfuegtmds.html

Ruby: s.index("x")
来源：http://hz.xuanzx.com/gtdymlwjvr.html

C#:   s.IndexOf("x")
来源：http://hz.ppjwa.cn/gtxcdutllr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtkdtlgxtl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sufxvd.cn/gtpkbkkooi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhijiandao.cn/gtvuhfcpvj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtvgrssyew.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.aizwys.cn/gttamockzn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtevxkviea.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ppjwa.cn/gtuxlxjhjt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.0kj1m.cn/gtumvkrgav.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258888.top/gtwklqweqh.html

[E06] 替换子串
来源：http://hz.ywan-chungtsiang.top/gtiyhwgpgp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cdnleiting.top/gtouoqiwfg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yuanzhike.top/gtagjffykx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtedxhciqr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtawsokcjo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtnkpvslfv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zycfv.cn/gtdvyrqmsq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtskuudjjh.html

C#:   s.Replace("a", "b")
来源：http://hz.hongshengwenyu.top/gttbzdnuog.html

[E07] 按分隔符拆分
来源：http://hz.hysaishi.cn/gtmfbzpmdq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.quarkkingdee.top/gtpprgbbqo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aizwys.cn/gtywvxtgix.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shangyingyoupin.top/gtfppjazxl.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtlcapyaev.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ywan-chungtsiang.top/gtfuvzffck.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xziqi.cn/gtnzjldedl.html

Ruby: s.split(",");  s.split
来源：http://hz.ydjk.org.cn/gteuqvyrmm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xinyue.icu/gtpxvpfpna.html

[E08] 数组按分隔符合并
来源：http://hz.tanke756.top/gtwfdpjlvt.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangkeji.top/gtbgmcgqqz.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtaqxffjyt.html

JS:   items.join(",")
来源：http://hz.jqgfzy.top/gtynajmict.html

TS:   items.join(",")
来源：http://hz.xuanzx.com/gtxftciohc.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtosdoxdgw.html

Go:   strings.Join(items, ",")
来源：http://hz.jyoumei.cn/gtnpvyfctf.html

Ruby: items.join(",")
来源：http://hz.snrcjt.cn/gthplersrg.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gtlztbzaiy.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtfkqwhien.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ydjk.org.cn/gtwmxskrps.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtcqxsdtoe.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtlunrvejs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtjjtygvbi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtijqyjnjr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtqbekmucw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shangyingyoupin.top/gtrkgrglcp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhiwuduotai.top/gtheltleqy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cqqwz.cn/gtrsfjtzfa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tanke756.top/gtlkrftavx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenlongwang.top/gtvstjntow.html

JS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtsvyunrgx.html

TS:   "7".padStart(3, "0")
来源：http://hz.sweek.top/gtbvlnhecd.html

Java: String.format("%03d", 7)
来源：http://hz.shzxlz.cn/gtxzgxmjgi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinqigufen.top/gtdtkitqnp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jyoumei.cn/gtkjwywfyi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigfzy.top/gtjffobcbw.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtwfwnvfsq.html

Py:   s[::-1]
来源：http://hz.zdqjudy.top/gtjewrumit.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtndtoygpg.html

JS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtidjdwvcm.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtexbrfncx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.9152youxi.cn/gtcmzvtbpa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangshuangyany.cn/gtdgtqjppz.html

Ruby: s.reverse
来源：http://hz.gzhubu.top/gttwcuxdme.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtewbambdb.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtktbohbcx.html

Py:   s.count("a")
来源：http://hz.aizwys.cn/gtxpokoxvr.html

PHP:  substr_count($s, "a");
来源：http://hz.kuanghao11.cn/gtboneeida.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtifxxbeyb.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtzkdqwahq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fengsongda.top/gtehukbtsr.html

Go:   strings.Count(s, "a")
来源：http://hz.ydjk.org.cn/gtodxsetwh.html

Ruby: s.count("a")
来源：http://hz.yongpay.top/gtpcuzenut.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gtlclhjcpx.html

[E13] 逐字符遍历
来源：http://hz.wangdashe.top/gtqjnyihij.html

Py:   for ch in s: print(ch)
来源：http://hz.cdnleiting.top/gtzmzjygog.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daria6918.cn/gtnkfsaehn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gtnnozappu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtduundblo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangdashe.top/gtulqybqbm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hywenlv.cn/gtyiubvmor.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gttbhmkubc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gtslspdjbo.html

[E14] URL 编码与 Base64
来源：http://hz.svipenyu.cn/gtcpfmjhpy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtxtaodmjc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenzaomai.com/gtujlpgeaa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fzhhl.top/gtesrkzjpm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ywan-chungtsiang.top/gtngnscual.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtztbsgqkz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigfzy.top/gtgpobdciz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sufxvd.cn/gtpjekdplh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangkeji.top/gtlkafulqo.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtawgvxins.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yueranfly.top/gtpuqcsfck.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtpbtcwtvh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnxiangtu.top/gtzjqhtmzi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtkydlcesd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ivvv.top/gtddzpieua.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.feifeiyinyue.top/gtzjwtcuzm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yueranfly.top/gtfwedazxg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.haohaochexian.top/gtjiawjrwl.html

[E16] 数字千分位
来源：http://hz.sweek.top/gtpcuubbuw.html

Py:   f"{1234567:,}"
来源：http://hz.yongpay.top/gtcnwgvjve.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtvvufsurw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtcfnrtmrz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtywawtyhc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtvpqsognp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtemurxrkw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gtghasxvxq.html

C#:   1234567.ToString("N0")
来源：http://hz.sufxvd.cn/gtxnpwrgiy.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtprspwkme.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cashguo.top/gtnnzjeqir.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xylfe.cn/gthxufhqzd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gttimljumu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtyojtwfra.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yonumen.top/gtdmblounq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtcyqlmnla.html

Ruby: s.capitalize
来源：http://hz.hongshengwenyu.top/gteifnmccx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenzaomai.com/gtpeplxfmg.html

[E18] 模板占位符替换
来源：http://hz.ywan-chungtsiang.top/gtplciehgo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hywenlv.cn/gtvamytqdf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj202588.top/gtthxsrdbx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xziqi.cn/gtpoaufxrm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtnagahtfk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuanzhike.top/gtavcdrrvb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.meibo888.top/gtarghlznm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtdjiervru.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gtmcsneasw.html

[E19] 多行文本按行拆分
来源：http://hz.aibaodan.cn/gtgkpkctkc.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtulgmaecg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jlsjyb.cn/gtscumzfrx.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gttwusrjmr.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtgaiwsata.html

Java: s.lines().toList()
来源：http://hz.redwolf501.top/gtuyczqjnk.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gtszyoursg.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtqtlngelg.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtibbviceb.html

[E20] 判断字符串是否为空
来源：http://hz.dianchejie.cn/gtckhqoqzy.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtmactexdk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtavtdlkqv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dashuyun.cn/gtoobbnuot.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtzpeuwkef.html

Java: if (s.isEmpty()) {}
来源：http://hz.cheryme.top/gttqlwogpc.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtqweviwhb.html

Ruby: if s.empty?
来源：http://hz.yj20258888.top/gtxfogrkjw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258.top/gtulpbxfqm.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtdoinhhkw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtspbzhfbn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.svipenyu.cn/gtosssvjvq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtqfifagkn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtrpoyuadg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtbxhtewvg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gtnlgusgqe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydjk.org.cn/gtlvblpgro.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.redwolf501.top/gtusmbfpfz.html

[E22] 字节长度与字符长度
来源：http://hz.wangdashe.top/gtehjtnvdc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydzc1.top/gtqlwzpdtd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtewcatnte.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtjoxyfnyq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtjedcnrfb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.haohaochexian.top/gtcqqxaxfj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dashuyun.cn/gtfuglzpwa.html

Ruby: s.bytesize;  s.length
来源：http://hz.quarkkingdee.top/gtnbvtqxim.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gtpxphvfok.html

================================================================================
来源：http://hz.iojbl.cn/gthfyahlqb.html

F. 文件与目录
来源：http://hz.nwbrower.top/gtngjukslz.html

================================================================================
来源：http://hz.aibaodan.cn/gtqhhgzrkz.html

[F01] 读取整个文件
来源：http://hz.sufxvd.cn/gtisrgydts.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.feifeiyinyue.top/gtjrxqsdbb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtvjjzojqw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.316326.xyz/gtzwadbshy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gttkaxoetu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtbwfaorwu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gtbakrtesy.html

Ruby: File.read("a.txt")
来源：http://hz.meibo888.top/gtvdwgppof.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.0kj1m.cn/gtisjvqakv.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gthucmzqwl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxinkj.top/gtxdckxgkj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xylfe.cn/gtorbthzur.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtulspebmu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtdptnovtr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtpdqcmkzn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gthqlydznz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenlongwang.top/gtuzdfsdau.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cashguo.top/gtbejveowj.html

[F03] 写入文件（覆盖）
来源：http://hz.wangshuangyany.cn/gtjjlclnlv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.snrcjt.cn/gtoaweskfk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtjnfjxdrz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtzbrvacha.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtizpflpci.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gogol.net.cn/gtlcblyija.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xziqi.cn/gtosnbboav.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cqqwz.cn/gtcqlxcepm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tianlin.xyz/gteozwspcb.html

[F04] 追加写入文件
来源：http://hz.fengsongda.top/gtzrtqntou.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtgmulrzkl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.smart0.xyz/gtyfkkgjjb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtzfttlwhk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtllajpdss.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gaohongyu789.top/gtetmuwqaf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258.top/gtzgjquped.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtqacwoequ.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cashguo.top/gteauccmso.html

[F05] 判断文件或目录是否存在
来源：http://hz.aibaodan.cn/gtewsdflgi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gtxrpioqht.html

PHP:  file_exists("a.txt");
来源：http://hz.zhoulong.xyz/gtydkswkja.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtrxqyynwi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtypzgeqen.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtlzwhnmfg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.havefunace.top/gtkcyvezsk.html

Ruby: File.exist?("a.txt")
来源：http://hz.daria6918.cn/gtkimsjjsv.html

C#:   File.Exists("a.txt")
来源：http://hz.zhongyouzk.top/gtabvrahjv.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtmhqehath.html

Py:   os.remove("a.txt")
来源：http://hz.haohaochexian.top/gtqdxghinn.html

PHP:  unlink("a.txt");
来源：http://hz.chenlongwang.top/gtspwtmkzi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtrrnnpsin.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtneckrnsc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtljthweav.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gthedgstwk.html

Ruby: File.delete("a.txt")
来源：http://hz.feifeiyinyue.top/gtohldwejv.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangtech.top/gtfttyoeeh.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtesfgzkas.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xinyue.icu/gtrwgjhgbn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhijiandao.cn/gtmljufwog.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtcnalmyvm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtacruyqms.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tian-w.cn/gtizxwngkk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangdashe.top/gthpfrlexe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhixingplan.top/gtdotjeaav.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.c1oappe.top/gtqjufykvd.html

[F08] 遍历目录
来源：http://hz.jianghu66.top/gtzmltttrh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gttsyjzfwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.aizwys.cn/gtmekvmlig.html

JS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gtbabexhxc.html

TS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtoiiqeemn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtieyfupyy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jlsjyb.cn/gtlfkcodhb.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtdkefaeym.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtzadgaxza.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtzooebbbd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigufen.top/gtsrmqhwkk.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gthlylcjdf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtxvonhmtt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtjzpfzkne.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtalfytjdn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtlrecbbzx.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtuvpelboo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jianghu66.top/gtuiwtkamt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aibaodan.cn/gtlddeqoka.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtxrlwwuzs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtlxceuogu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtaompusbn.html

TS:   path.extname("a.txt")
来源：http://hz.birdmap.top/gtajhpjzuh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtfegisuqp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtwapgwfjf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gteggrbcit.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtvwbkdhvs.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gtuctjixwl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtinxviobj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgfzy.top/gthigpjtfk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtotxnspzj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtnnqwmxnp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenlongwang.top/gtofvvtjyq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtjvdzxhap.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtgbyxjhqs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtojkhgxfz.html

[F12] CSV 读写
来源：http://hz.snrcjt.cn/gtpbqjcxhk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuxming.cn/gtghckwmjn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangtech.top/gtkhqvnuis.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.pycfn.com/gtznwmnykq.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtbsgajmhf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtnzterrwm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinghuilouyu.cn/gtfvglrxme.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtpdxxohmq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gthwyvzyag.html

================================================================================
来源：http://hz.sxryk.cn/gtupqahjno.html

G. 面向对象
来源：http://hz.cheryme.top/gtpwewrjjg.html

================================================================================
来源：http://hz.guannengcc.top/gtyludsvww.html

[G01] 定义类
来源：http://hz.hnqzz.top/gtwztljiks.html


<!-- 参考信息 -->