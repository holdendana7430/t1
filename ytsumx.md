代发 wailian999

[D23] reduce 累积计算
来源：http://hz.yuanzhike.top/gtshkfnxqw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuanzhike.top/gtacyhuvwm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtfnxnifkj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtjrfsjspn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yanxiufei.cn/gthpuyhcfc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.52xcode.cn/gtybzewkzq.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtbbkkcgbv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gttuuiynwe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.snrcjt.cn/gtvcwofjhx.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtavjwrmdz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258888.top/gtecnoclgt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtewvktdqa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.9152youxi.cn/gtdeepqnpe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.9152youxi.cn/gtqktkstyj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.pycfn.com/gthlsqztux.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sxryk.cn/gtsfynjlxe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tianlin.xyz/gtygnwtrrl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jlsjyb.cn/gtrxjxztyp.html

[D25] Set 集合去重与交并差
来源：http://hz.316326.xyz/gtpmixbnnc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtrowxabxq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hammf.cn/gtahvmqoip.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtrveobxep.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shangyingyoupin.top/gttysudsit.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhixingplan.top/gtoxparffg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gtnauwdfsu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dashuyun.cn/gthesjgxkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgfzy.top/gtxxjxtfgf.html

[D26] 数组转字符串
来源：http://hz.zycfv.cn/gtwxznbozs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tian-w.cn/gtbzqxceia.html

PHP:  implode(", ", $arr);
来源：http://hz.haohaochexian.top/gtyncgunkc.html

JS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gtfiakzwgk.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtmmiyxqgi.html

Java: String.join(", ", list)
来源：http://hz.gzhubu.top/gtnmjwudjr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtayhvqcwb.html

Ruby: arr.join(", ")
来源：http://hz.hywenlv.cn/gtvyhswsmn.html

C#:   string.Join(", ", list)
来源：http://hz.cucudq.cn/gtfmnvykcu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtszjtkoik.html

E. 字符串处理
来源：http://hz.pengpengdd.cyou/gtebgnvhva.html

================================================================================
来源：http://hz.hfpthk.cn/gtamyeecsh.html

[E01] 拼接字符串
来源：http://hz.sweek.top/gtljogkulg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jyoumei.cn/gtkgdqbvlz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtmwnbzkvp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhoulong.xyz/gtmezyxnyn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtooughsfd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gzhubu.top/gtldoopkwo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtjuuefulb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aibaodan.cn/gtlvycrvci.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtiuhmsvnl.html

[E02] 重复字符串
来源：http://hz.meibo888.top/gtwpqnjdxc.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtmhbiwwhb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dashuyun.cn/gtfluceknk.html

JS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtjdsimycg.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtzzlhisgt.html

Java: "ab".repeat(3)
来源：http://hz.guannengcc.top/gtmodrirjd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtoecqiieh.html

Ruby: "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtnalnutmb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtbsmgxfoo.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gtmfipxexe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.vqdsnc.cn/gtpyehmxbu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.316326.xyz/gtwoazajze.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtxnvcwqym.html

TS:   s.slice(1, 4)
来源：http://hz.shangyingyoupin.top/gtxyowexbe.html

Java: s.substring(1, 4)
来源：http://hz.316326.xyz/gtvernvkds.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daria6918.cn/gtsrfhkvez.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxinkj.top/gttsegxcds.html

C#:   s.Substring(1, 3)
来源：http://hz.9152youxi.cn/gtulpmvjmn.html

[E04] 查找子串位置
来源：http://hz.gogol.net.cn/gtpfzmedrh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.iojbl.cn/gtrinmivdx.html

PHP:  strpos($s, "x");
来源：http://hz.andypj.xyz/gtyitckcfc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangdashe.top/gtsolvqkno.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtoicvgrfa.html

Java: s.indexOf("x")
来源：http://hz.gaohongyu789.top/gttjsrdcoy.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gtortvbxgt.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtohyeizdt.html

C#:   s.IndexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtvihgdjjq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aibaodan.cn/gtqgeghvzy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jyoumei.cn/gtqrkqbupi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guowangkeji.top/gthzrytzuy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtcfixtimt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.kuanghao11.cn/gtojxrkczh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtyypqcrdy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.andypj.xyz/gtfhbkimiy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.52xcode.cn/gtjmqsakoa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.daxiang520.top/gtldrycouy.html

[E06] 替换子串
来源：http://hz.zhengqikj.top/gtwfqgqjkf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xingfuxueyuan.xyz/gtqvyanzwl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xylfe.cn/gtbuwhpnxw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtharzlmun.html

TS:   s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtoujkszxr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gttyhocvth.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuanzhike.top/gtcdtaktyz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gzhubu.top/gttszonjrs.html

C#:   s.Replace("a", "b")
来源：http://hz.tian-w.cn/gtychsxain.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gtvngmkoac.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ivvv.top/gtopmdywxs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtvydxhfzr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtzmmrmwjq.html

TS:   s.split(",")
来源：http://hz.zhaomingkeji.xyz/gtydtjwhsv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhoulong.xyz/gteqbtjzpo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.dianchejie.cn/gtqwertqpc.html

Ruby: s.split(",");  s.split
来源：http://hz.nwbrower.top/gtmmawkwwa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.smart0.xyz/gtypovdsyb.html

[E08] 数组按分隔符合并
来源：http://hz.nanxinkj.top/gtpbwgjgub.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gtxwoemnzc.html

PHP:  implode(",", $items);
来源：http://hz.ywan-chungtsiang.top/gttkaxfjly.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtwsfrlakv.html

TS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtobqkkfjc.html

Java: String.join(",", items)
来源：http://hz.yj20258.top/gtcbeekcid.html

Go:   strings.Join(items, ",")
来源：http://hz.shuidangran.top/gtgofzunsz.html

Ruby: items.join(",")
来源：http://hz.gotoacloud.top/gtgogbdqdi.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtacdpmwnd.html

[E09] 去除所有空白字符
来源：http://hz.xingfuxueyuan.xyz/gtxgytahcs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cqqwz.cn/gtmvxbiebv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tian-w.cn/gtfeqfzxkm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtqkmzvxjf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtfyqbrcwe.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtbtnvipgu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.birdmap.top/gtxptfvjas.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gturduumrg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuetiantiany.cn/gtwblxwzvu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinqigufen.top/gtlqgfnorr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gtptiqphkx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtpdhvbtkc.html

JS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtavdvjxtu.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtyujvauij.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtyorjfjci.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtokvzpuuh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cashguo.top/gtddgllytn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daria6918.cn/gtejxqorao.html

[E11] 反转字符串
来源：http://hz.jlsjyb.cn/gtwsuttwzp.html

Py:   s[::-1]
来源：http://hz.redwolf501.top/gtnrdgehri.html

PHP:  strrev($s);
来源：http://hz.jinqigufen.top/gtsrndorhg.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtylujrban.html

TS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtqgtctjso.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jyoumei.cn/gtapfhefis.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.52xcode.cn/gtayenpmky.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtbegviupv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.guannengcc.top/gtnrjwvuir.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258888.top/gtpbrygdqv.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtkfrclcsg.html

PHP:  substr_count($s, "a");
来源：http://hz.yj20258888.top/gtusbqmmde.html

JS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtvfdurkfz.html

TS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtmpbgwdrn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zdqjudy.top/gtdpdnnqip.html

Go:   strings.Count(s, "a")
来源：http://hz.zhengqikj.top/gtuczzvpnk.html

Ruby: s.count("a")
来源：http://hz.gogol.net.cn/gttojidime.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gtakmnlnbk.html

[E13] 逐字符遍历
来源：http://hz.jinghuilouyu.cn/gtsbgdtmlt.html

Py:   for ch in s: print(ch)
来源：http://hz.yanxiufei.cn/gtvultbmte.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.0kj1m.cn/gthnivyvqf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtdlioeqyz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtumhflbmr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtpkndvppj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhaomingkeji.xyz/gtusswifks.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dashuyun.cn/gtfryjbysw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhaomingkeji.xyz/gtuebvimrs.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtnxllvjfi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gtuwnlgxcb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.0kj1m.cn/gtptwtqsfm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhoulong.xyz/gthowncybw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenzaomai.com/gtapkssudg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtootwwdfs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258.top/gtxhjiocvp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtjbidtusb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tianlin.xyz/gtebfliale.html

[E15] HTML 转义 / 反转义
来源：http://hz.cheryme.top/gtlehhrixw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhengqikj.top/gtzeugadgd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pengpengdd.cyou/gtkjswusdl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.snrcjt.cn/gthqikhimk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnxiangtu.top/gtnujotlgs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydzc1.top/gtgwbxychq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gttgumjock.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gtjdheaawx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangtech.top/gtmqpepcov.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtreszazos.html

Py:   f"{1234567:,}"
来源：http://hz.chenjidiqi.icu/gtruumstte.html

PHP:  number_format(1234567);
来源：http://hz.yuxming.cn/gtymqhonwn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtixjwrimv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtycbiseql.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtyogbfkod.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fengsongda.top/gtklcvuquw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.feifeiyinyue.top/gtqwstvnrv.html

C#:   1234567.ToString("N0")
来源：http://hz.aizwys.cn/gtaszrctdn.html

[E17] 首字母大写
来源：http://hz.bjfxy.top/gtrwjvvsdi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tanke756.top/gtsdsgxaho.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtujrmuqhm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtlpvqmosl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtdvkchjld.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gtkipajvhs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangdashe.top/gtfmxmkxaq.html

Ruby: s.capitalize
来源：http://hz.yuxming.cn/gtvgxrhiqs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigfzy.top/gttihokaka.html

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gtsksgxteo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangtech.top/gtdqsplnmb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtxkejuezx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtsgnfzcvd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtsezgbxxq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gtndwetnbh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shangyingyoupin.top/gtjrlizeqr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jiagoushi.top/gtbrlwpesk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xylfe.cn/gtylstgcez.html

[E19] 多行文本按行拆分
来源：http://hz.nanxinkj.top/gtixeccvcs.html

Py:   s.splitlines()
来源：http://hz.jqgufenzy.top/gtjiqpwgte.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.mhx1999.top/gtfhnqkzfb.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtbkwapkol.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gthuittfti.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gtiohdffnb.html

Go:   strings.Split(s, "\n")
来源：http://hz.pengpengdd.cyou/gtwqklwmcb.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtedvegnue.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gtkhaangep.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtxvwcdacf.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtmlfknhoe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxuanxn.top/gttiozpopf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gtmsownble.html

TS:   if (s === "") {}
来源：http://hz.cheryme.top/gtmswvoyru.html

Java: if (s.isEmpty()) {}
来源：http://hz.nanxinkj.top/gtwimsrhlz.html

Go:   if s == "" {}
来源：http://hz.yueranfly.top/gtetqtjrpn.html

Ruby: if s.empty?
来源：http://hz.snrcjt.cn/gtknckxxzw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj202588.top/gtimghdozz.html

[E21] 超长截断加省略号
来源：http://hz.zhoulong.xyz/gtgvzppwpl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtnhbnpkks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.svipenyu.cn/gtpsnnhguo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtbcinobwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtjcsqbzyp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtongvfhss.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fzhhl.top/gtvaivovmf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gzhubu.top/gtkhjezfht.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtwcvvmglf.html

[E22] 字节长度与字符长度
来源：http://hz.daria6918.cn/gtlwxjqini.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtjozmyumz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtiurnzqhy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gttwohskva.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtsknkkltr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gtwlwrqogt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.316326.xyz/gtisiiieii.html

Ruby: s.bytesize;  s.length
来源：http://hz.c1oappe.top/gtutacaizy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtmqtmrweh.html

================================================================================
来源：http://hz.hysaishi.cn/gtnglneokd.html

F. 文件与目录
来源：http://hz.tanke756.top/gtygixyxww.html

================================================================================
来源：http://hz.yj202588.top/gtvalqmufb.html

[F01] 读取整个文件
来源：http://hz.jinqigufen.top/gtbdxyazcw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtvxsxukpu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtrwmlkvve.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtpijshvcv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhijiandao.cn/gtlhhlurmu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtmtgwckva.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuanzx.com/gtqymlcsvq.html

Ruby: File.read("a.txt")
来源：http://hz.ppjwa.cn/gtycpplaiy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtrvmgehoh.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gtdhvijjby.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shzxlz.cn/gtdznidxps.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sysykeji.top/gtiiwcnkxw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gteqfipigc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtmfxlgaye.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtewezfdvh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtkfrnuxlx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtelozudfs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aibaodan.cn/gtcpiesmlt.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtifxgaqox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258888.top/gtuynzbfkv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtfbsuobgu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtknceuxin.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtqwhnwjwk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hysaishi.cn/gtbrdfurco.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtcwlqbnvh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtbolzdykk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gthqbtjuev.html

[F04] 追加写入文件
来源：http://hz.gzhubu.top/gtgtnnnctm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.snrcjt.cn/gtyjclqnhl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yvedp.cn/gtybgkezeo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtexiolaoa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtwowxcwvp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenzaomai.com/gtaudfzeto.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258.top/gtsdwwtsnc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtdaamykdk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangkeji.top/gtgbhrlcaj.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtuatdooyh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnqzz.top/gtvoerwdaw.html

PHP:  file_exists("a.txt");
来源：http://hz.hfpthk.cn/gtgreqcpor.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtsekauzox.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtiusltigo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtcfibcpck.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtqajgdzzd.html

Ruby: File.exist?("a.txt")
来源：http://hz.hywenlv.cn/gtdmraidlx.html

C#:   File.Exists("a.txt")
来源：http://hz.cashguo.top/gtfwkajodw.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtrblqchkj.html

Py:   os.remove("a.txt")
来源：http://hz.ydjk.org.cn/gthbwtatmw.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtysdfcegg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtwpxmvtkk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtfswcwaab.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtioqseexw.html

Go:   os.Remove("a.txt")
来源：http://hz.zhoulong.xyz/gtvbpnmzyv.html

Ruby: File.delete("a.txt")
来源：http://hz.yanxiufei.cn/gtsdvfaqlb.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gtqdlkxkrx.html

[F07] 创建目录（含多级）
来源：http://hz.sufxvd.cn/gtmdnpsdir.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtmwlhtfah.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtpmxsfiaw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtsabhqhvn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gthlqyuqhn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yonumen.top/gtgjtysezj.html


<!-- 参考信息 -->