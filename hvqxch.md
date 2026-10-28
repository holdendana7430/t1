代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtpszjvoop.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.iojbl.cn/gtuiezxmtv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gtuhfszadf.html

TS:   [...arr];
来源：http://hz.zhongyouzk.top/gtkornypwu.html

Java: new ArrayList<>(list);
来源：http://hz.nwbrower.top/gthlbwyqvk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtgvcjnlvg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jiagoushi.top/gtkrtbyrjm.html

C#:   new List<int>(list);
来源：http://hz.zdqjudy.top/gtgqpbtgvv.html

[D23] reduce 累积计算
来源：http://hz.birdmap.top/gttpvvivgp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gttszwnslg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yongpay.top/gtfzacpnpq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gttsiaggdq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtgrndkkoq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gteiwigwnb.html

Go:   // 手写循环
来源：http://hz.ydzc1.top/gtkrvpefdb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jianghu66.top/gthjeunyzg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ivvv.top/gttbonukmx.html

[D24] 字典 / Map 基本操作
来源：http://hz.pycfn.com/gtcczkaxqh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dianchejie.cn/gtwnrluwat.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtbmpfzgej.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gtkrosuzke.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sufxvd.cn/gtpdsgipri.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yangfankeji.com/gtavgdyddz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.feifeiyinyue.top/gtlsyixsjk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.vqdsnc.cn/gtubqoisuz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtfavoijag.html

[D25] Set 集合去重与交并差
来源：http://hz.yanxiufei.cn/gtsflwfdhg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtfgwktprp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.redwolf501.top/gtcfwmldia.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtrvxcjvot.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cheryme.top/gtrbjzpxcg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gtsoeanftl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tian-w.cn/gtjcarrzmw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yanxiufei.cn/gtygstfnyx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj202588.top/gtfgbpdicj.html

[D26] 数组转字符串
来源：http://hz.zdqjudy.top/gtejryapzj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jiagoushi.top/gthlxckstz.html

PHP:  implode(", ", $arr);
来源：http://hz.hnxiangtu.top/gthsuriuvw.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtmqnyxenx.html

TS:   arr.join(", ")
来源：http://hz.yj20258.top/gtgndpumdh.html

Java: String.join(", ", list)
来源：http://hz.gaohongyu789.top/gtyfqbxdiv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtuhltlcll.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtmqocjtcn.html

C#:   string.Join(", ", list)
来源：http://hz.aibaodan.cn/gtnwngpnvc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrxtmyebb.html

E. 字符串处理
来源：http://hz.ppjwa.cn/gtjfteziqe.html

================================================================================
来源：http://hz.havefunace.top/gtwhekufhh.html

[E01] 拼接字符串
来源：http://hz.xuanzx.com/gtldwvdtcd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtobhyrcrg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xylfe.cn/gtzofajmnk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtnggqacgk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gttdvopfxq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jiagoushi.top/gtsgtywkom.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cheryme.top/gtyahfuhub.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydjk.org.cn/gtjtiqhzti.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtrzbyonhs.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtfifljjnf.html

Py:   "ab" * 3
来源：http://hz.shangyingyoupin.top/gtxpptbvhu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nwbrower.top/gtkoheccfa.html

JS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtrrwikdiq.html

TS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtmmlchvlk.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtdysrvyga.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tian-w.cn/gtxsqpezxu.html

Ruby: "ab" * 3
来源：http://hz.jqgfzy.top/gtlaboctng.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuanzhike.top/gtzxvmdiiy.html

[E03] 截取子串
来源：http://hz.smart0.xyz/gtjunhjtqx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigfzy.top/gtvhrqtizx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtroparjhl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtfuzewqku.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtiwdcprpb.html

Java: s.substring(1, 4)
来源：http://hz.guannengcc.top/gtgnlqfabb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.smart0.xyz/gtnxmbrjjp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj20258888.top/gtbgkvccny.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gtajhnniwn.html

[E04] 查找子串位置
来源：http://hz.tanke756.top/gtshzwjorp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jlsjyb.cn/gteqgiynui.html

PHP:  strpos($s, "x");
来源：http://hz.zhijiandao.cn/gtbllthumd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenzaomai.com/gthknmjypp.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gtncosyrlm.html

Java: s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtwrbkjfnq.html

Go:   strings.Index(s, "x")
来源：http://hz.yonumen.top/gtwtmecsah.html

Ruby: s.index("x")
来源：http://hz.xuetiantiany.cn/gtrfvxlkip.html

C#:   s.IndexOf("x")
来源：http://hz.mhx1999.top/gtseltemcj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jiagoushi.top/gtruftmqtl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuetiantiany.cn/gtrctnozdc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gttykhvcwf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yongpay.top/gtroytadeb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jianghu66.top/gtslaqtwam.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtmdgdssoe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zdqjudy.top/gtolqdopwi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtbssgbydy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtsvvnmjzv.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gtwvmdibyd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gtmjfwoaiy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sxryk.cn/gtsefbgdlv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtlhuenuqn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtobwrxpar.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtwrvojwje.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jlsjyb.cn/gtemacofjs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtdnfktfpi.html

C#:   s.Replace("a", "b")
来源：http://hz.kuanghao11.cn/gtrudzftpe.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gtxsdvhpgd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.0kj1m.cn/gtaxtsqgui.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tianlin.xyz/gtqcdbjnvk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtfoscpqji.html

TS:   s.split(",")
来源：http://hz.yj20258888.top/gtcubsmjwi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.9152youxi.cn/gtvzmukmze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.kuanghao11.cn/gtpvwzlzsd.html

Ruby: s.split(",");  s.split
来源：http://hz.smart0.xyz/gtiomfmfqp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dashuyun.cn/gtqlkrydwt.html

[E08] 数组按分隔符合并
来源：http://hz.shangyingyoupin.top/gtiomuqeqb.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtksheinnq.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtdukjchcn.html

JS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtorkpsalq.html

TS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtihodkoss.html

Java: String.join(",", items)
来源：http://hz.shangyingyoupin.top/gtdzurpzbn.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtqwyrnobg.html

Ruby: items.join(",")
来源：http://hz.shzxlz.cn/gtxddaurja.html

C#:   string.Join(",", items)
来源：http://hz.shuidangran.top/gtepmjjgwv.html

[E09] 去除所有空白字符
来源：http://hz.sxryk.cn/gtyqbljyow.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gtvueqifly.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.mhx1999.top/gtejuvarnr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtrbbxvhph.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtterarlcb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sweek.top/gtqqyxvgwr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yueranfly.top/gtowipuxtm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yanxiufei.cn/gtxkoqykqx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangtech.top/gtcltdphdv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.svipenyu.cn/gtpweqcpkf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.aizwys.cn/gthpoprfbb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gtibhestmi.html

JS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtqqimjxvt.html

TS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtiaumzaii.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtsdblkpli.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258888.top/gtxodyvuzt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtalrwycsl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jyoumei.cn/gtcrfucems.html

[E11] 反转字符串
来源：http://hz.meibo888.top/gtemubjelv.html

Py:   s[::-1]
来源：http://hz.smart0.xyz/gtsofvweox.html

PHP:  strrev($s);
来源：http://hz.shzxlz.cn/gtbnkeljnr.html

JS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtcanymcll.html

TS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtnmdwwolb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.c1oappe.top/gtoaafhqeo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yueranfly.top/gtgfoydtub.html

Ruby: s.reverse
来源：http://hz.meibo888.top/gtaycqjvkg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtltaqafwh.html

[E12] 统计某字符出现次数
来源：http://hz.xylfe.cn/gtqrjmlycw.html

Py:   s.count("a")
来源：http://hz.jinqigufen.top/gtdkxqjvdg.html

PHP:  substr_count($s, "a");
来源：http://hz.ivvv.top/gtpztkcgzy.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtniqnmabo.html

TS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtkrpkclvi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gtyqbfmnpi.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258888.top/gturupzmnj.html

Ruby: s.count("a")
来源：http://hz.shangyingyoupin.top/gtiwnvczhw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gttymcmscq.html

[E13] 逐字符遍历
来源：http://hz.dashuyun.cn/gtqftjttoi.html

Py:   for ch in s: print(ch)
来源：http://hz.hammf.cn/gtfisivfws.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.andypj.xyz/gtkgqurmqx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtexihzpxo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtqlvxmfql.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ivvv.top/gtgvvsrqxn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yanxiufei.cn/gtughcruda.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuanzx.com/gtrrsiqecz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gzhubu.top/gtblsywogk.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gtnhrberwz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.vqdsnc.cn/gtgucbffmg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydjk.org.cn/gtheabpvnu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pengpengdd.cyou/gtxdzudrgz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sysykeji.top/gtyegiqbnf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yongpay.top/gthrftrllo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hnqzz.top/gtoopclgbw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pengpengdd.cyou/gtvbfhjrsx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtoqgbrrdv.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigfzy.top/gtnutwoeuk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gthunbynep.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhijiandao.cn/gtqcfeqajr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtcgvbznev.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhixingplan.top/gtdkmlvkdi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtcozrvnnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.mhx1999.top/gtbryrtwqp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenzaomai.com/gtndijrpkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenjidiqi.icu/gtuzqtlyoj.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtvnldtnsr.html

Py:   f"{1234567:,}"
来源：http://hz.yvedp.cn/gtssrvbdxl.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtjrfcndvh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtaayxruyg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtydxzxgqi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtnrfkctql.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xinyue.icu/gtxwyawvyj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sweek.top/gtnjfnatgm.html

C#:   1234567.ToString("N0")
来源：http://hz.fzhhl.top/gteewqyfxo.html

[E17] 首字母大写
来源：http://hz.yonumen.top/gtgolefhkl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.haohaochexian.top/gtxtmpzers.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtmiacnvpu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtcwqlshth.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtplfkkgxw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tanke756.top/gtbvqtjcxi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gttwcgsztp.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtlugklqxu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtxgldmdrg.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gthdwzslfo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zdqjudy.top/gtojhbidae.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hongshengwenyu.top/gtsopenqjq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtdohhiixw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtfyciwdwm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtypddroey.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.vqdsnc.cn/gthuuemyll.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cucudq.cn/gtybizhmyz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258.top/gtqhwjowke.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtubgtlurg.html

Py:   s.splitlines()
来源：http://hz.guowangkeji.top/gtwqujwrpu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gtfbuxfcnk.html

JS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gtuiipiogz.html

TS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtyoeroxcl.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtgxuiuwft.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenzaomai.com/gtsauwlehw.html

Ruby: s.lines
来源：http://hz.wangshuangyany.cn/gtfxosdkka.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gteuvopreu.html

[E20] 判断字符串是否为空
来源：http://hz.52xcode.cn/gthnlhwesk.html

Py:   if not s:
来源：http://hz.cheryme.top/gtkqmhukyt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgufenzy.top/gtjiqbjlee.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtkcscircj.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gtcrrulqot.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtmzcfqjsd.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gtotziomfh.html

Ruby: if s.empty?
来源：http://hz.zdqjudy.top/gtclvjbejl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gttkcxrsvk.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gtgdylmmls.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cqqwz.cn/gtpxjyuixu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.9152youxi.cn/gtpcxgvjmn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtzjuiqeye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtbhtjppqr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtibyomeyw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zycfv.cn/gtrouvvwbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yonumen.top/gtmtshxdkl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtekanewme.html

[E22] 字节长度与字符长度
来源：http://hz.redwolf501.top/gtioipeoxd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtukvwfhdh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtgpqyvqhf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtzhbwyldh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtrwwguvst.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cashguo.top/gtairsdfwq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtpayujilq.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnxiangtu.top/gtfycrhtma.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gtlahprjee.html

================================================================================
来源：http://hz.yueranfly.top/gtfsisofrc.html

F. 文件与目录
来源：http://hz.316326.xyz/gtmziaxlav.html

================================================================================
来源：http://hz.zhixingplan.top/gtndrpefsh.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtswcjioln.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shangyingyoupin.top/gtpkeoasrw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuetiantiany.cn/gtktbyluji.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtfhktmxkx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxinkj.top/gtlvrncgdg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gthcxulsnj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.snrcjt.cn/gtzbbdxnwq.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtjtatvlou.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtlmtqynzu.html

[F02] 逐行读取文件
来源：http://hz.yvedp.cn/gtculjilxh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gtayahksny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.meibo888.top/gtpmjmbhao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtgbmuimcz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtqijmppcq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtmtzggjoj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gthwthmttq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.andypj.xyz/gtaoghxacx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtwjcqxooc.html

[F03] 写入文件（覆盖）
来源：http://hz.ydzc1.top/gtlbqzxnzw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigfzy.top/gtfuwostww.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtjwyildld.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtmhcqyuei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtnrekhqrr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtqhrviakl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtvepibvkj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hfpthk.cn/gtelftsatr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydzc1.top/gtbibuplzq.html

[F04] 追加写入文件
来源：http://hz.cdnleiting.top/gtoxpkrukf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gttjljovns.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtcrezaxgy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangshuangyany.cn/gtifjfcexy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtqfnbhgnq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangtech.top/gtllbpjxvc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yongpay.top/gtnyeofiae.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtkjwujdpe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.9152youxi.cn/gtyfniyrfa.html

[F05] 判断文件或目录是否存在
来源：http://hz.gogol.net.cn/gtzusofroh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aizwys.cn/gtinaajoxq.html

PHP:  file_exists("a.txt");
来源：http://hz.xziqi.cn/gtdcjhokfu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtsyrjlnmp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtpkgljdhy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtvngmxsnl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.svipenyu.cn/gtkkikxqni.html

Ruby: File.exist?("a.txt")
来源：http://hz.gogol.net.cn/gtrsomoaui.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtojzhrnfm.html

[F06] 删除文件
来源：http://hz.aibaodan.cn/gtvetllhtp.html

Py:   os.remove("a.txt")
来源：http://hz.ydjk.org.cn/gtjnnvaxxo.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtzncefjyq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtcmsypywd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtiqlalion.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtgogvrvrx.html

Go:   os.Remove("a.txt")
来源：http://hz.quarkkingdee.top/gtgzsgmruk.html


<!-- 参考信息 -->