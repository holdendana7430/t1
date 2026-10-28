代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gthjkwnjxg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guowangkeji.top/gtigasxqhm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gzhubu.top/gtqgfzmzvn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.mhx1999.top/gtjkyjsiiz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nwbrower.top/gttnoxqzle.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yongpay.top/gtxeeubmda.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtqbfdizhr.html

[D26] 数组转字符串
来源：http://hz.jinqigfzy.top/gtdxubkyao.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhijiandao.cn/gtbunckpti.html

PHP:  implode(", ", $arr);
来源：http://hz.hnqzz.top/gtizjrkpor.html

JS:   arr.join(", ")
来源：http://hz.ivvv.top/gtzlkvoabl.html

TS:   arr.join(", ")
来源：http://hz.meibo888.top/gtnzkxvlfl.html

Java: String.join(", ", list)
来源：http://hz.jqgufenzy.top/gtffqqvpxb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtfazwbcjn.html

Ruby: arr.join(", ")
来源：http://hz.vqdsnc.cn/gtgmxgdsod.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gthhfnfare.html

================================================================================
来源：http://hz.chenlongwang.top/gthbuepxgg.html

E. 字符串处理
来源：http://hz.havefunace.top/gtbucgkiaf.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtufjkgbdg.html

[E01] 拼接字符串
来源：http://hz.chenjidiqi.icu/gtpubbejnc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtxkzjzjix.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangtech.top/gtaigzokmk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtxwmarwfb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtlosrhudq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.wangshuangyany.cn/gtqqtlgnoy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuanzx.com/gtytsyagpa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj202588.top/gtptmwylql.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtaazbffcu.html

[E02] 重复字符串
来源：http://hz.chenjidiqi.icu/gtjkkivuug.html

Py:   "ab" * 3
来源：http://hz.ivvv.top/gtbiaqfvfn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnqzz.top/gtuycfrrgl.html

JS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtspzcyhre.html

TS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtymxumwhl.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtslgacimx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinghuilouyu.cn/gtsikvnhtb.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtfedzvgam.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtfzixfpfe.html

[E03] 截取子串
来源：http://hz.ppjwa.cn/gtgyyhlfjm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtwmfflxzf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtxxbxmski.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuanzx.com/gtglwcukgv.html

TS:   s.slice(1, 4)
来源：http://hz.nwbrower.top/gtlcfjkcji.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtgxhssnpl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yongpay.top/gtedanszwi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gtnlhlngtd.html

C#:   s.Substring(1, 3)
来源：http://hz.tanke756.top/gtddlluzls.html

[E04] 查找子串位置
来源：http://hz.sufxvd.cn/gtlnuacluj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cdnleiting.top/gtfpyieorx.html

PHP:  strpos($s, "x");
来源：http://hz.zhoulong.xyz/gtxcmvzmui.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxuanxn.top/gtvsxtjrro.html

TS:   s.indexOf("x")
来源：http://hz.ydjk.org.cn/gtebuzovyn.html

Java: s.indexOf("x")
来源：http://hz.gotoacloud.top/gtfohcctdi.html

Go:   strings.Index(s, "x")
来源：http://hz.ydzc1.top/gtwbkhbuwv.html

Ruby: s.index("x")
来源：http://hz.yj20258888.top/gtokcoorka.html

C#:   s.IndexOf("x")
来源：http://hz.nwbrower.top/gttigjrvpn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aizwys.cn/gtqlksebsn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.vqdsnc.cn/gtnygjhqeh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gaohongyu789.top/gttyqxnlpk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtwarcrswr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtrjzfctah.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtkhzjjswg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ppjwa.cn/gtlvuqjhoy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenzaomai.com/gtmkizodpy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xylfe.cn/gtgloomkur.html

[E06] 替换子串
来源：http://hz.kuanghao11.cn/gtgrfbbnyk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gthqowolzf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.bjfxy.top/gtkmsdompo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtrbxdtzpl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtsmwnifan.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gthbllyboq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.c1oappe.top/gtkyotsoiw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtvkhhamxk.html

C#:   s.Replace("a", "b")
来源：http://hz.pycfn.com/gtjrcqpjcu.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtxuoarpcx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gteqjttoca.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gtipuktcmm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fengsongda.top/gtukdswpeg.html

TS:   s.split(",")
来源：http://hz.iojbl.cn/gtnybzteiz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ppjwa.cn/gtxqfysmmx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtjmeqkokp.html

Ruby: s.split(",");  s.split
来源：http://hz.cdnleiting.top/gtqnphucfu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydjk.org.cn/gtktwbgzvs.html

[E08] 数组按分隔符合并
来源：http://hz.0kj1m.cn/gtvitgrleu.html

Py:   ",".join(items)
来源：http://hz.ppjwa.cn/gteehmvvno.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtklvaspzs.html

JS:   items.join(",")
来源：http://hz.tianlin.xyz/gtmgklfdod.html

TS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtesnkhkgc.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gtonhyvtuk.html

Go:   strings.Join(items, ",")
来源：http://hz.hysaishi.cn/gtupfvjjar.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gtruwwpyop.html

C#:   string.Join(",", items)
来源：http://hz.ydzc1.top/gtgqaeafvm.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtzlxpevbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtqgbsihwd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhixingplan.top/gtqdzqihqs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gogol.net.cn/gtpfzanens.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtoknhquxn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuxming.cn/gtefiwedvg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gtwivywvvw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dianchejie.cn/gtirceqfdf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuxming.cn/gtguaxowji.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtkqgqvskq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gttodlsjns.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fengsongda.top/gtrekgxcpz.html

JS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtuvizmxup.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gternnhtil.html

Java: String.format("%03d", 7)
来源：http://hz.ydzc1.top/gtinbzfxca.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtgnyzipek.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gttzvfuaax.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dashuyun.cn/gtmgpbbemz.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtgndubgvn.html

Py:   s[::-1]
来源：http://hz.52xcode.cn/gtwzvwhesh.html

PHP:  strrev($s);
来源：http://hz.yanxiufei.cn/gtobtwmvej.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtlojlropq.html

TS:   [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtgxpbektq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gtgbatzxin.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xinyue.icu/gtguanlbwl.html

Ruby: s.reverse
来源：http://hz.xziqi.cn/gtmnbpyuvd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtntkptqha.html

[E12] 统计某字符出现次数
来源：http://hz.aibaodan.cn/gtmwwafvlr.html

Py:   s.count("a")
来源：http://hz.sxryk.cn/gtoltsvcba.html

PHP:  substr_count($s, "a");
来源：http://hz.zhoulong.xyz/gtrquivtgp.html

JS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtjmhwuylb.html

TS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtakohcric.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.haohaochexian.top/gtubjdzult.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gtvzdguqsa.html

Ruby: s.count("a")
来源：http://hz.ydjk.org.cn/gtwilzives.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtbfkudvdo.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtrccgdpda.html

Py:   for ch in s: print(ch)
来源：http://hz.meibo888.top/gtbvktltbu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hysaishi.cn/gtpocbejxq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtatebwtlz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hysaishi.cn/gtdtouyrfn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258888.top/gtapnmmphg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ppjwa.cn/gtsoqnasiy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xylfe.cn/gttwerjpjj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258888.top/gtfzbtlagg.html

[E14] URL 编码与 Base64
来源：http://hz.pengpengdd.cyou/gtttgtfkrk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangkeji.top/gtxrgowehf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gtocrcgdxr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gttpbfwlrw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.0kj1m.cn/gtpikpnccb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.316326.xyz/gtkqlfpgpg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhixingplan.top/gtugndswij.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yanxiufei.cn/gthtaugqsm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.c1oappe.top/gtjlweqvhj.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigfzy.top/gtsxeymids.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gaohongyu789.top/gtjpdglqzb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hfpthk.cn/gtadhjtmig.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuanzx.com/gtpmbxbmzu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtkmppvgpu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtazppmtsx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.snrcjt.cn/gtvdyjqkke.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhengqikj.top/gteyngugxh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gthfkfnjzn.html

[E16] 数字千分位
来源：http://hz.ybcxt.top/gtfggpnnei.html

Py:   f"{1234567:,}"
来源：http://hz.fzhhl.top/gtmfqwazaq.html

PHP:  number_format(1234567);
来源：http://hz.iojbl.cn/gtlrtmveif.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pycfn.com/gtbjymxizd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtzrfxvfqw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gotoacloud.top/gtbvijefto.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtnfxxcvsp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yueranfly.top/gtvbmkpenv.html

C#:   1234567.ToString("N0")
来源：http://hz.jinghuilouyu.cn/gtlzyhvvsj.html

[E17] 首字母大写
来源：http://hz.yonumen.top/gtgaaldrto.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtmpfzxnga.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yanxiufei.cn/gtntoiipkl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtyvbobkhr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtmuwjyguh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtgmjptbnv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tanke756.top/gtpqtkjybs.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtapixugvm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gtspjiiapy.html

[E18] 模板占位符替换
来源：http://hz.smart0.xyz/gteeygemmw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtculolpdj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtkrlydrek.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gttaomaojx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtaoxfyxir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.pengpengdd.cyou/gtwneflicd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtuqorswej.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinghuilouyu.cn/gtwmpaotck.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtdynijfqk.html

[E19] 多行文本按行拆分
来源：http://hz.gogol.net.cn/gtrknduyla.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtvhpcljkr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gthnwwophs.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtdqftbeaq.html

TS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtvkuwqyjo.html

Java: s.lines().toList()
来源：http://hz.ybcxt.top/gtourhhmmq.html

Go:   strings.Split(s, "\n")
来源：http://hz.daria6918.cn/gtebkwsngz.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gtizzizlot.html

C#:   s.Split('\n')
来源：http://hz.daria6918.cn/gthlxsttfk.html

[E20] 判断字符串是否为空
来源：http://hz.jinyuanbaomall.cn/gtmhvzxihf.html

Py:   if not s:
来源：http://hz.dashuyun.cn/gtgayrnvhs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnqzz.top/gtkccpkwbz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xinyue.icu/gtpaowjvoo.html

TS:   if (s === "") {}
来源：http://hz.yueranfly.top/gtqotvgxmw.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtosxmqxnu.html

Go:   if s == "" {}
来源：http://hz.hnxiangtu.top/gtvdwicmrf.html

Ruby: if s.empty?
来源：http://hz.ybcxt.top/gtjznxfkwu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gtbsrphdfc.html

[E21] 超长截断加省略号
来源：http://hz.jinyuanbaomall.cn/gtevkuhmuf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgfzy.top/gtlkkuyurj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shangyingyoupin.top/gtevkbcxyd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gthaajzahu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtewomsoel.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtrjpqhyaq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtnkfcnzyt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hfpthk.cn/gtuyucenib.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtjodjhvyu.html

[E22] 字节长度与字符长度
来源：http://hz.zhongyouzk.top/gtrgjobgvv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guowangkeji.top/gttxsbfriu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtnvgqmpkj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtmsgfonch.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtittbzdmq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.andypj.xyz/gtvwlvvouj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtsecjdynm.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhoulong.xyz/gtssvksavl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xylfe.cn/gtcgodbmoo.html

================================================================================
来源：http://hz.smart0.xyz/gtzddgjqgt.html

F. 文件与目录
来源：http://hz.yonumen.top/gtwgwsgoer.html

================================================================================
来源：http://hz.zhengqikj.top/gtteaemfhe.html

[F01] 读取整个文件
来源：http://hz.sysykeji.top/gtpuomltfe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhengqikj.top/gtnjoigzat.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shuidangran.top/gtpkliqxbb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gtpdcneumv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gaohongyu789.top/gtqmggzyxl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtqwgwwgad.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtwmkzftjp.html

Ruby: File.read("a.txt")
来源：http://hz.daxiang520.top/gtwiduoqri.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtdacppyfi.html

[F02] 逐行读取文件
来源：http://hz.shangyingyoupin.top/gtzjkihcna.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xylfe.cn/gtumcwfsjp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtelovmdvz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtuxlnnvww.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gtmhitvcht.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtfppivlui.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtwtyynavu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guannengcc.top/gtaqliodkm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.haohaochexian.top/gtsrkrzauw.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtpvxzwhos.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtxwliqmmx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ybcxt.top/gtqthvfabw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daxiang520.top/gtbtzpohqo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtrwpykqhz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigfzy.top/gtzcrgvsrs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinghuilouyu.cn/gtjfyonwnn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daxiang520.top/gttverxtxm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fzhhl.top/gtnabmceqq.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtisixlurk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.c1oappe.top/gtjhpbtflm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtzamomkjk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtxxgirggu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtudcndfms.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtpwrrqygc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtluuojmhn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gtbfwossid.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtzktlrtjm.html

[F05] 判断文件或目录是否存在
来源：http://hz.sysykeji.top/gtithymtid.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinghuilouyu.cn/gtpvupqjrh.html

PHP:  file_exists("a.txt");
来源：http://hz.yangfankeji.com/gtakmtnmig.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtzdjehtzq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtandrcvrq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gthdmjmnqs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gtngqfrolk.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigufen.top/gtnncmoabh.html

C#:   File.Exists("a.txt")
来源：http://hz.hysaishi.cn/gtckcogzoc.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtcocwsgic.html

Py:   os.remove("a.txt")
来源：http://hz.yj202588.top/gttiabpuap.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtgbuazsrr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtrahbplvv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtxhrbumdl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtjkhixbpw.html

Go:   os.Remove("a.txt")
来源：http://hz.zycfv.cn/gtrqjbroas.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gtaaigltcn.html

C#:   File.Delete("a.txt");
来源：http://hz.ybcxt.top/gtwbmfpeci.html

[F07] 创建目录（含多级）
来源：http://hz.yonumen.top/gthrknpqfk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtczhjaoxy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtjzliogsc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtjekimpba.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtmatqpeqm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shuidangran.top/gtxddbqlmr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinghuilouyu.cn/gtgoehsssg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtvobiulep.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtnazcfeik.html

[F08] 遍历目录
来源：http://hz.sweek.top/gtuezcbgpd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtarsfxkej.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gtgczmbprg.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gttmvezqze.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtlklenxby.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtjlsouezf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenzaomai.com/gtuzdmmuok.html

Ruby: Dir.children("dir")
来源：http://hz.chenlongwang.top/gtxouhamlx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtlrpnonoc.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtqzjwwqxe.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinghuilouyu.cn/gtxorqncfv.html

PHP:  filesize("a.txt");
来源：http://hz.chenjidiqi.icu/gtmusqglux.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtrxfjkfqh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtvqnlulpm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtptfibtsv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nwbrower.top/gtdkjugxyi.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtpxpewliq.html


<!-- 参考信息 -->