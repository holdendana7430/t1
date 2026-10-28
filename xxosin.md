代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtdofrqbwx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenjidiqi.icu/gtbvgcqcvr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ybcxt.top/gtrjructvz.html

C#:   new List<int>(list);
来源：http://hz.ybcxt.top/gtlaffjwqx.html

[D23] reduce 累积计算
来源：http://hz.iojbl.cn/gtitmytren.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gogol.net.cn/gtzdclnwnj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daria6918.cn/gtuvtybggj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gtgjetmjfa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtwojgwrjj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258888.top/gtlumjnxto.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtsgsfikcg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtmrfezpgg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtcbpzjjpe.html

[D24] 字典 / Map 基本操作
来源：http://hz.zycfv.cn/gtjlkahlyf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zdqjudy.top/gtbxzftvbj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtzbrnsjaa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hongshengwenyu.top/gtlyufxwao.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtmjyywkxh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gtlcyqkwnx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.meibo888.top/gtgyfnctfo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuetiantiany.cn/gtuxipnwlk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hywenlv.cn/gtqwdfegdm.html

[D25] Set 集合去重与交并差
来源：http://hz.guannengcc.top/gtqkelwnto.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jiagoushi.top/gtkzaxhyww.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtnhemhgbh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sxryk.cn/gtalkegaty.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtwtfuayhs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.redwolf501.top/gtmqjohxvl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gtivcrgshm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtxqhwrscm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhiwuduotai.top/gtsvdtghsr.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtiafrvpot.html

Py:   ", ".join(map(str, arr))
来源：http://hz.havefunace.top/gtnmoxvawk.html

PHP:  implode(", ", $arr);
来源：http://hz.chenzaomai.com/gtvhfptzof.html

JS:   arr.join(", ")
来源：http://hz.ivvv.top/gtjmwntcus.html

TS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtugljdbtu.html

Java: String.join(", ", list)
来源：http://hz.fengsongda.top/gtqmqztypw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhiwuduotai.top/gttwbuozje.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtwwinsdas.html

C#:   string.Join(", ", list)
来源：http://hz.zhixingplan.top/gtxbqezmcg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqvabukwy.html

E. 字符串处理
来源：http://hz.jinqigfzy.top/gtvsgjcdmb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtpvpmxfkx.html

[E01] 拼接字符串
来源：http://hz.zhengqikj.top/gtkemfwipn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tanke756.top/gtdqherqhx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.bjfxy.top/gtierpnmsl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtfbmsdltg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtpjijmmpn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.vqdsnc.cn/gtuezhdgys.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ehwqpu.com/gtlgcwryxz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sufxvd.cn/gtpwcuroqy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gttiwqcfeg.html

[E02] 重复字符串
来源：http://hz.tanke756.top/gtmuxpkkmj.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtifbwjxdf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.vqdsnc.cn/gtvwtqwlzh.html

JS:   "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtccwniqyb.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gteynwheza.html

Java: "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtofkcwecz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigfzy.top/gtqblagjdo.html

Ruby: "ab" * 3
来源：http://hz.52xcode.cn/gtzvyybwzb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yvedp.cn/gticgmmvzs.html

[E03] 截取子串
来源：http://hz.andypj.xyz/gtohtmbepf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangshuangyany.cn/gtotfyfxxu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj202588.top/gthfkxrsga.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtxsnvtsps.html

TS:   s.slice(1, 4)
来源：http://hz.jyoumei.cn/gtbyvqiimn.html

Java: s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtxowutxgp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxuanxn.top/gtvcracwrl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sweek.top/gtpgunqbpr.html

C#:   s.Substring(1, 3)
来源：http://hz.hfpthk.cn/gtantdudix.html

[E04] 查找子串位置
来源：http://hz.xuetiantiany.cn/gtsgluzvzl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zdqjudy.top/gtriyqvphh.html

PHP:  strpos($s, "x");
来源：http://hz.snrcjt.cn/gtccksoprf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinqigfzy.top/gtcuqedyie.html

TS:   s.indexOf("x")
来源：http://hz.jinqigufen.top/gtcaxtbbvw.html

Java: s.indexOf("x")
来源：http://hz.zhoulong.xyz/gtpwccusze.html

Go:   strings.Index(s, "x")
来源：http://hz.zycfv.cn/gtgntmpmog.html

Ruby: s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtxfotvana.html

C#:   s.IndexOf("x")
来源：http://hz.sxryk.cn/gtmgxsbxvb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnxiangtu.top/gtmkudxguf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.redwolf501.top/gtigiiuzqa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtuqcgjbtd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtxnpufmqb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.mhx1999.top/gtvhkalwbw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gttgwbmhrc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yueranfly.top/gtgwlblpqw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zdqjudy.top/gtszguzbsz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.snrcjt.cn/gtqzwehijv.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtwvbzonla.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xylfe.cn/gtiqtodako.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sxryk.cn/gtqskkwghl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtunjaoobn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtwwhhexlv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtrkdiofpj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yueranfly.top/gtaakgnhyv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxinkj.top/gtnfepklnd.html

C#:   s.Replace("a", "b")
来源：http://hz.yonumen.top/gtyfmoldnz.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtesqungdp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gthvvanjci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgfzy.top/gtpjxwyyde.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.havefunace.top/gttozefaxt.html

TS:   s.split(",")
来源：http://hz.zhaomingkeji.xyz/gtjjsnlsqt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cdnleiting.top/gtvaurfqec.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jianghu66.top/gtvafthiyt.html

Ruby: s.split(",");  s.split
来源：http://hz.aizwys.cn/gtvofsxyku.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.haohaochexian.top/gtqplbkqlk.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gthkqpeioo.html

Py:   ",".join(items)
来源：http://hz.yuanzhike.top/gtxkgjxyfk.html

PHP:  implode(",", $items);
来源：http://hz.xziqi.cn/gtypauqcfa.html

JS:   items.join(",")
来源：http://hz.yangfankeji.com/gtlmwytvch.html

TS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtabwhbcde.html

Java: String.join(",", items)
来源：http://hz.tanke756.top/gtpfzolijb.html

Go:   strings.Join(items, ",")
来源：http://hz.chenlongwang.top/gtfloblvuz.html

Ruby: items.join(",")
来源：http://hz.yuxming.cn/gtqqizuojr.html

C#:   string.Join(",", items)
来源：http://hz.wangdashe.top/gtljwywnuv.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtsbxoztsm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gtdkvsqpab.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.fzhhl.top/gtplwoenea.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtvkwirvqm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtkzvkbedb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aizwys.cn/gtaltysyxi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cdnleiting.top/gtirczgtcg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gtwlatzmln.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenzaomai.com/gtmzeyemhr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zdqjudy.top/gtywpoppdk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtpwxyrppu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xingfuxueyuan.xyz/gthlvgkudf.html

JS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtroqqpkvy.html

TS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtourppvjc.html

Java: String.format("%03d", 7)
来源：http://hz.sxryk.cn/gthpuyqxwa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sxryk.cn/gtcdumncvp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gtwvwjjnsc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtubsyeabt.html

[E11] 反转字符串
来源：http://hz.sxryk.cn/gticvjrhzd.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gttmdkidoq.html

PHP:  strrev($s);
来源：http://hz.yj20258888.top/gtcryokpsf.html

JS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtegqzlbox.html

TS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtajuzruqy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnxiangtu.top/gtvalvaaki.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ywan-chungtsiang.top/gtkptesqxv.html

Ruby: s.reverse
来源：http://hz.jyoumei.cn/gtsdulqowj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtxgiqzsgr.html

[E12] 统计某字符出现次数
来源：http://hz.sysykeji.top/gtusihpepg.html

Py:   s.count("a")
来源：http://hz.quarkkingdee.top/gtimvxxdxo.html

PHP:  substr_count($s, "a");
来源：http://hz.cheryme.top/gtnrxckxrd.html

JS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtldrbrcdl.html

TS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtfrxlxobu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.haohaochexian.top/gtqeagfjes.html

Go:   strings.Count(s, "a")
来源：http://hz.tianlin.xyz/gtltajegwr.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtkojanmnc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtcitjobdt.html

[E13] 逐字符遍历
来源：http://hz.yj202588.top/gtmywspmyo.html

Py:   for ch in s: print(ch)
来源：http://hz.yonumen.top/gtpowokrsm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gotoacloud.top/gtidcqvybh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtmutmigtq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhijiandao.cn/gtmbdyjksy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhijiandao.cn/gtnslbdnck.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xylfe.cn/gtlmfvhgap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtkqoipopu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gthfryhyjc.html

[E14] URL 编码与 Base64
来源：http://hz.tianlin.xyz/gtlbzkdhtc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.iojbl.cn/gttydqgpra.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhaomingkeji.xyz/gtisvnclrd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtrkuxvytb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gteewqxbyo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.iojbl.cn/gtydbbbbwt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tianlin.xyz/gtslombrxg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.smart0.xyz/gtperroosz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xinyue.icu/gtduwsqepn.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenjidiqi.icu/gtbzaxgnqe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenlongwang.top/gtrkbodsqw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ivvv.top/gtyumrxfcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guannengcc.top/gtbpaynrxi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydjk.org.cn/gttucggzeo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ivvv.top/gtlybthdil.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xylfe.cn/gtlddfyauq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cdnleiting.top/gtbkpuqlyt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hfpthk.cn/gtbjjtpfje.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gtmobnskqr.html

Py:   f"{1234567:,}"
来源：http://hz.jyoumei.cn/gttpbjusfa.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtjltaxtto.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtutdodmum.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtutbtwcqy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhongyouzk.top/gteanubzef.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jqgufenzy.top/gtbsziitib.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cashguo.top/gtdlbatcbg.html

C#:   1234567.ToString("N0")
来源：http://hz.tanke756.top/gteptkwlch.html

[E17] 首字母大写
来源：http://hz.fengsongda.top/gtoytcbuob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.daxiang520.top/gtzkfkhqyn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cashguo.top/gtidhmvtss.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtwgxrsxqc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fengsongda.top/gtfklndgff.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtysjsnoru.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gtmmvcmdec.html

Ruby: s.capitalize
来源：http://hz.chenjidiqi.icu/gtnnrypzjc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xziqi.cn/gtvsjlbghw.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gtqoidmopt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtpqpttwco.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.smart0.xyz/gthcsujjdr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtfgcdqzjh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtqwhaypnp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zycfv.cn/gtlsldqqbu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtrwljbewa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtblolrgkq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhaomingkeji.xyz/gtmuthksjy.html

[E19] 多行文本按行拆分
来源：http://hz.smart0.xyz/gtliuuiisv.html

Py:   s.splitlines()
来源：http://hz.gzhubu.top/gtpxndgjen.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtgwkorhel.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtipxdhofg.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gthjlkhdrx.html

Java: s.lines().toList()
来源：http://hz.kuanghao11.cn/gtrvrwadqc.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtccnjdxco.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtyjfqvhai.html

C#:   s.Split('\n')
来源：http://hz.zhengqikj.top/gtylxqjwbv.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gturwkbmql.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gtqdrxhmut.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jyoumei.cn/gtuyeocfiv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhoulong.xyz/gtkhxaptcc.html

TS:   if (s === "") {}
来源：http://hz.fzhhl.top/gttokvmxih.html

Java: if (s.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtczydjltz.html

Go:   if s == "" {}
来源：http://hz.pengpengdd.cyou/gtpzzsitbw.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtukbczual.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtwfsnonxf.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtuetmmili.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnxiangtu.top/gtqnrlosky.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yvedp.cn/gtmpawceod.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtcxykyuxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtdvidtzed.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtwoklffhm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tian-w.cn/gtrxkzzpqu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.c1oappe.top/gtqpymjqdv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sufxvd.cn/gtdredrwoa.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258888.top/gtyxevmbyi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtufcwxmdn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gthajcjfkb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtqyfxwugg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtzqpwqatb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yueranfly.top/gtrtodmbfe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pengpengdd.cyou/gtsxuzfywn.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtfnczfdih.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtebniiupj.html

================================================================================
来源：http://hz.cqqwz.cn/gtlrrfxwvd.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gtmdfavavr.html

================================================================================
来源：http://hz.shuidangran.top/gtcibyehvj.html

[F01] 读取整个文件
来源：http://hz.sweek.top/gtnnalhwvy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fzhhl.top/gtwddzktuc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtjegqdqua.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhaomingkeji.xyz/gtzivqpewf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xinyue.icu/gtpqtpauha.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtmsbrlmiy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxinkj.top/gtqoewqbqs.html

Ruby: File.read("a.txt")
来源：http://hz.fengsongda.top/gtxkpgmkuw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtgnduvmjw.html

[F02] 逐行读取文件
来源：http://hz.jqgfzy.top/gttwxxkcnq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtoquuxggc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cqqwz.cn/gtyblymerz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtwkxhedde.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtaxokzdzh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtoccfzzyz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yangfankeji.com/gtyqkrdtzm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hysaishi.cn/gtympfouom.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ywan-chungtsiang.top/gtkrghsipc.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtuojdxlve.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.52xcode.cn/gttbosmkev.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gthyskmkgv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtlpxsrgas.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtfubspdla.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gtpgszukmh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aibaodan.cn/gtgvlcyxfq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtluwleyvy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtkpwrdesk.html

[F04] 追加写入文件
来源：http://hz.pengpengdd.cyou/gtgjisyckd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gtgmixqfbm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtcoentbxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gthbvxijaj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtktgmqjgg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnqzz.top/gtstetfrzw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258.top/gtldaxzvid.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.mhx1999.top/gtdjcxfnue.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yanxiufei.cn/gteoowyhgs.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxinkj.top/gtxmbzlzhf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.meibo888.top/gtikzmpjia.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258.top/gtlilqxwvk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtgjfgqtzy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtdqhlaczf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtrtskacod.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtdaijnwut.html

Ruby: File.exist?("a.txt")
来源：http://hz.yvedp.cn/gtwgcltrzh.html

C#:   File.Exists("a.txt")
来源：http://hz.gaohongyu789.top/gtyxdrqyyl.html

[F06] 删除文件
来源：http://hz.wangdashe.top/gtupxsnoee.html

Py:   os.remove("a.txt")
来源：http://hz.hammf.cn/gtemnjcsrr.html

PHP:  unlink("a.txt");
来源：http://hz.cucudq.cn/gtcbiouhxr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtauekaurx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtmpjsdmnb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gttywhvdbi.html

Go:   os.Remove("a.txt")
来源：http://hz.jiagoushi.top/gtromylstf.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtmmjkgwsj.html

C#:   File.Delete("a.txt");
来源：http://hz.gotoacloud.top/gtrrtilnil.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtvcfxduwd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gtzcvriglj.html


<!-- 参考信息 -->