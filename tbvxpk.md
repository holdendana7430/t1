代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gtdtohkgot.html

[D24] 字典 / Map 基本操作
来源：http://hz.tian-w.cn/gtiomqbepy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtzkpeercx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.aizwys.cn/gtgpmqcdcj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydzc1.top/gtdienqvkv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.316326.xyz/gtlbvisnha.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtodgbznaw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuanzhike.top/gtpkjupomo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guannengcc.top/gtyhshzcte.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenzaomai.com/gtpxloqywu.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtgakrhlll.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.0kj1m.cn/gtxpzluntb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtmuabwluy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daria6918.cn/gtgkqniiht.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gtiacplvnu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.mhx1999.top/gtwizhmerq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cucudq.cn/gtnctduqgp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jiagoushi.top/gtvrhmnnhf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtjedzbslw.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtkvkcmnhz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtqsevkxtg.html

PHP:  implode(", ", $arr);
来源：http://hz.svipenyu.cn/gtzsbzwlvj.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtmjybjqok.html

TS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtdeiyrvwe.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtfzkbrliq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtaljcbdda.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtyxlmxifb.html

C#:   string.Join(", ", list)
来源：http://hz.cashguo.top/gttkfzdcuy.html

================================================================================
来源：http://hz.snrcjt.cn/gtyxqgtlkn.html

E. 字符串处理
来源：http://hz.c1oappe.top/gtrrzhoejc.html

================================================================================
来源：http://hz.zdqjudy.top/gthrrotegw.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtpxuqxuvk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgufenzy.top/gtnisuxbtw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cheryme.top/gtlutbdnyo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtgnhmsjld.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.52xcode.cn/gtejlnzbvm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinghuilouyu.cn/gtnmknynhl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtptqptbjg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yvedp.cn/gtmqsoldam.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtjhzndexu.html

[E02] 重复字符串
来源：http://hz.havefunace.top/gtuwlehvkt.html

Py:   "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gttifmwpxb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aibaodan.cn/gtldecumii.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtrpzvpxnu.html

TS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtirkznleg.html

Java: "ab".repeat(3)
来源：http://hz.ybcxt.top/gtanhoqtks.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ppjwa.cn/gtrelpzxpw.html

Ruby: "ab" * 3
来源：http://hz.zycfv.cn/gtntvuflqm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhaomingkeji.xyz/gtgxwyzltt.html

[E03] 截取子串
来源：http://hz.wangshuangyany.cn/gtbmyfjxod.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.andypj.xyz/gtswclrdgn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigufen.top/gtupygqnti.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtqiitsvkz.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtisfciuwb.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtchtpnqkp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.wangdashe.top/gtzitbbclx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gtoobfwugb.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtijssxwes.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtcweouwvu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zdqjudy.top/gtyzgxlobw.html

PHP:  strpos($s, "x");
来源：http://hz.kuanghao11.cn/gtcxgocdgq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj202588.top/gticavmvsi.html

TS:   s.indexOf("x")
来源：http://hz.zhoulong.xyz/gtbksetltd.html

Java: s.indexOf("x")
来源：http://hz.bjfxy.top/gtbkvhkbgm.html

Go:   strings.Index(s, "x")
来源：http://hz.chenzaomai.com/gtvtpadbpn.html

Ruby: s.index("x")
来源：http://hz.zycfv.cn/gtivqglmcf.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtiyermlku.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jianghu66.top/gtpjqhcata.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xylfe.cn/gtcpevaffj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sysykeji.top/gtcgqqnncg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtcxdyxdff.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangshuangyany.cn/gtzkhzfwsm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtfqvxeyat.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.0kj1m.cn/gtzprsdpov.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangdashe.top/gtndevtjph.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.feifeiyinyue.top/gtzosgyhxr.html

[E06] 替换子串
来源：http://hz.jianghu66.top/gtoteqjhmy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guannengcc.top/gtgoblspmx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtijhkjxax.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtremcywev.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gturhavpxc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtwjekxfwa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.bjfxy.top/gtbrrootes.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtsrmwsauz.html

C#:   s.Replace("a", "b")
来源：http://hz.svipenyu.cn/gtfuldxejb.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtybexbyfa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ivvv.top/gtrerfeuid.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgufenzy.top/gttyyhbtif.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xziqi.cn/gtohjyzigz.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtgcvehatz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zycfv.cn/gtvnazzxly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gtfqoqpvoy.html

Ruby: s.split(",");  s.split
来源：http://hz.zhoulong.xyz/gtjckisgji.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shanyushiyangkeji.top/gtkzhuexgm.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtfoeqspha.html

Py:   ",".join(items)
来源：http://hz.gogol.net.cn/gtabenplxp.html

PHP:  implode(",", $items);
来源：http://hz.zhaomingkeji.xyz/gtwuzphpda.html

JS:   items.join(",")
来源：http://hz.jiagoushi.top/gtrjgqbqga.html

TS:   items.join(",")
来源：http://hz.zhaomingkeji.xyz/gtawjjznva.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gtubvfvcrd.html

Go:   strings.Join(items, ",")
来源：http://hz.nwbrower.top/gtkbgfaxcq.html

Ruby: items.join(",")
来源：http://hz.aizwys.cn/gtbpwpfuzs.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtucvcdjut.html

[E09] 去除所有空白字符
来源：http://hz.chenjidiqi.icu/gtykienrpj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtxspwzjhw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pycfn.com/gtvgofzwuh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtqrqmcxbo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtvjiewipn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.52xcode.cn/gtleilrysa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xziqi.cn/gtmbeugunx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtsvfyzclq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtcqajtnbz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtxnfoxfmj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtqccrpvuw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxinkj.top/gtevkfcjik.html

JS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gttcfzfrzh.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtuahawtyv.html

Java: String.format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtsyofinxd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtdkkaqiss.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtgqnmapve.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yonumen.top/gtdindlywy.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gtfauyzpwu.html

Py:   s[::-1]
来源：http://hz.gzhubu.top/gtififvtkn.html

PHP:  strrev($s);
来源：http://hz.hnxiangtu.top/gtqpkdsfsl.html

JS:   [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtuzsuhjvm.html

TS:   [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtbahwwdix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinghuilouyu.cn/gtemuxsqjz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.iojbl.cn/gtcijieidp.html

Ruby: s.reverse
来源：http://hz.xuetiantiany.cn/gtpdqztgvo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtkyrbifqf.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtnpwrxrei.html

Py:   s.count("a")
来源：http://hz.dianchejie.cn/gtevkzegsz.html

PHP:  substr_count($s, "a");
来源：http://hz.zhongyouzk.top/gtvnvtonir.html

JS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtzailpayu.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtriynqnyq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtmihkjway.html

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gtmvanopfd.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtrfmrpiyk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sufxvd.cn/gtoaoyhejb.html

[E13] 逐字符遍历
来源：http://hz.zdqjudy.top/gtpoqpuzvm.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtccdbrmoh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigufen.top/gthdyjufeh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtuhiwlmrk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gtqfwioptu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtwlhdvjnr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtdqyvvcgr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtlgpznors.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.quarkkingdee.top/gtvpflbgcw.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtqglpgnev.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yvedp.cn/gtnlkshvyv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtbpndvayg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hammf.cn/gtfvxsyeeq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pycfn.com/gtwzlrexan.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydzc1.top/gtodqefnvl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangtech.top/gtklvdvwty.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.0kj1m.cn/gttsdkfydb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtovnjniag.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gtdoatxxih.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.birdmap.top/gtwlzjkccv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhijiandao.cn/gtunexsukk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jlsjyb.cn/gtpkwiuick.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtlbhvqrwy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yanxiufei.cn/gtcvjpmpzg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.snrcjt.cn/gtajziqoof.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aizwys.cn/gtxzlpuabf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guannengcc.top/gtdqnamthc.html

[E16] 数字千分位
来源：http://hz.pycfn.com/gtqqfzosza.html

Py:   f"{1234567:,}"
来源：http://hz.ydjk.org.cn/gtlqztvfqa.html

PHP:  number_format(1234567);
来源：http://hz.nwbrower.top/gtzlkjacrv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtxireloxl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtndefpfvq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yongpay.top/gtbunggcel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ppjwa.cn/gttqmzbgcb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tanke756.top/gtvqhioeoe.html

C#:   1234567.ToString("N0")
来源：http://hz.daxiang520.top/gttseapujj.html

[E17] 首字母大写
来源：http://hz.yonumen.top/gtelfwthve.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtppuobgri.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yangfankeji.com/gtxvaiubvg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtkiopovqf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtvlaogpew.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guowangkeji.top/gtkjbhtooh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtiwlvbmip.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtulnbpqxg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gtevbnmlnk.html

[E18] 模板占位符替换
来源：http://hz.hywenlv.cn/gtngxcycvl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenlongwang.top/gtcopxaraq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuetiantiany.cn/gttqnwheyt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtecellocu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gthsrzmfdw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gthrvbjykz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shzxlz.cn/gteicxtqrm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sufxvd.cn/gtvjwzxsxl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.316326.xyz/gtpxplalhn.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gtpwkrkkwu.html

Py:   s.splitlines()
来源：http://hz.hfpthk.cn/gtrtaqxovc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtgpmfyxqc.html

JS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtfhedymvy.html

TS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtypfytduj.html

Java: s.lines().toList()
来源：http://hz.andypj.xyz/gtazckzrto.html

Go:   strings.Split(s, "\n")
来源：http://hz.guannengcc.top/gtgbzuyosq.html

Ruby: s.lines
来源：http://hz.mhx1999.top/gtnezeuvga.html

C#:   s.Split('\n')
来源：http://hz.zhaomingkeji.xyz/gtbwjsjwsg.html

[E20] 判断字符串是否为空
来源：http://hz.zhaomingkeji.xyz/gtlxdozevq.html

Py:   if not s:
来源：http://hz.ppjwa.cn/gtciibkxzo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ppjwa.cn/gtttiiglsv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtpfzxrnwf.html

TS:   if (s === "") {}
来源：http://hz.kuanghao11.cn/gthfoqrofo.html

Java: if (s.isEmpty()) {}
来源：http://hz.cashguo.top/gtoczoeftc.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtkpqgucel.html

Ruby: if s.empty?
来源：http://hz.sufxvd.cn/gthognodvn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtgejnsbis.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtegdolmps.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gteuxzsdvj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gteyypvssz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtslrkqvnc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtkfvbpfyh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtwqnqlrjm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtawhedniv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gogol.net.cn/gtobmvmivy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.9152youxi.cn/gtwpswybgj.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtlbhlgeuo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.meibo888.top/gtzhqjbhgg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtgfsfrsfk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtmlnuhssu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gttmvqqlrf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnqzz.top/gttgaxofzk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jyoumei.cn/gtjnucvdsn.html

Ruby: s.bytesize;  s.length
来源：http://hz.sweek.top/gtvqhynjan.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xylfe.cn/gtnyytfcpp.html

================================================================================
来源：http://hz.yj20258.top/gtpzsxdkfz.html

F. 文件与目录
来源：http://hz.dianchejie.cn/gttkttcyqa.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfufdmgbn.html

[F01] 读取整个文件
来源：http://hz.xziqi.cn/gthqdwehtz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtxapajcow.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jyoumei.cn/gtvkholgtm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gtczjshjps.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhijiandao.cn/gtymvcbxws.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtjhtnvpwi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtoqfctwgc.html

Ruby: File.read("a.txt")
来源：http://hz.shzxlz.cn/gtqfglfktr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yongpay.top/gtmsxnftxt.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gtwbcjakbd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yongpay.top/gtzznvbszs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.feifeiyinyue.top/gtgwnekwto.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtglilxuza.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtdmvewqrq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtjycnkafw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dianchejie.cn/gtgmedzhke.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtjiuerplc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.havefunace.top/gtpzyqwlzg.html

[F03] 写入文件（覆盖）
来源：http://hz.havefunace.top/gtvdmrutij.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gzhubu.top/gtdvshdvfm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtycuwtxfo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtxpabnwlz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtaotdxluf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.iojbl.cn/gtfmaxzyvy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hfpthk.cn/gtpbboheee.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pycfn.com/gtcicdkkww.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gteajtpoxc.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtkhbygves.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhaomingkeji.xyz/gtpjxutjdf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhengqikj.top/gttcukgeho.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtndktnuhl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtdzfezugl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.iojbl.cn/gtwjjfrunm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtavengjux.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ybcxt.top/gtscwyajev.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhiwuduotai.top/gtpxsqarhg.html

[F05] 判断文件或目录是否存在
来源：http://hz.52xcode.cn/gthgksfaii.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtomfjeeck.html

PHP:  file_exists("a.txt");
来源：http://hz.xziqi.cn/gterylmdgg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtharigwtg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtdygkrkyc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtewcfnnbc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhengqikj.top/gtvtkjmppk.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtscspovkl.html

C#:   File.Exists("a.txt")
来源：http://hz.tian-w.cn/gtheyfjizw.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtlbvxpomr.html

Py:   os.remove("a.txt")
来源：http://hz.hywenlv.cn/gthsonbwoh.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtaxyavakf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpzjbwwwz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtlmuxjxxs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtdvokkclf.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtyfcovcpc.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtmfhntqfd.html

C#:   File.Delete("a.txt");
来源：http://hz.cheryme.top/gtniskswqh.html

[F07] 创建目录（含多级）
来源：http://hz.yanxiufei.cn/gttadllnds.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gtxtzmaisb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangkeji.top/gtmtltwlqp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtfsorxcxu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtngeoutqk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuanzhike.top/gttupmadvx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jyoumei.cn/gthfhutpfz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtnpmhqfhq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxuanxn.top/gtddbayaaa.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gtwjjsoebh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtznesjpyd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gtvhekanoq.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtpdhblnco.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gthijjyvhr.html


<!-- 参考信息 -->