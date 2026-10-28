代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gturpmvadf.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtdsvqxvyh.html

C#:   list.Contains(x)
来源：http://hz.0kj1m.cn/gtsxvtvbca.html

[D22] 复制数组（避免共享引用）
来源：http://hz.dianchejie.cn/gtthrftuny.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.andypj.xyz/gtwbxsgvbe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtkorvapst.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ybcxt.top/gtruuqrjvn.html

TS:   [...arr];
来源：http://hz.pycfn.com/gtirhmqqtp.html

Java: new ArrayList<>(list);
来源：http://hz.xziqi.cn/gtnjwajfhn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinyuanbaomall.cn/gtkvzotljr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtotovbpzc.html

C#:   new List<int>(list);
来源：http://hz.jinyuanbaomall.cn/gtqwpzutex.html

[D23] reduce 累积计算
来源：http://hz.bjfxy.top/gtwrkkadyi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigfzy.top/gtcaghfkxi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dianchejie.cn/gtrmwvodqo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtzvhfjles.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtjnpnvfzp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtdkabrxhl.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtsfnvztek.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtndhzltph.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daria6918.cn/gtehowtfip.html

[D24] 字典 / Map 基本操作
来源：http://hz.feifeiyinyue.top/gtyfgoeojc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cashguo.top/gttyfdpjds.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhaomingkeji.xyz/gteprnludv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtwkmnzruk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.vqdsnc.cn/gtqocrxksj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zycfv.cn/gtcfbcomkc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gaohongyu789.top/gtqypllpol.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtdafsdjyi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.c1oappe.top/gtfyxoeafc.html

[D25] Set 集合去重与交并差
来源：http://hz.hammf.cn/gtekqgjixf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gthsuieqzq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shangyingyoupin.top/gtdxkznanp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtsnjcyikr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hfpthk.cn/gtnknkbruc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtoozxqwus.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ppjwa.cn/gtzdwytrdg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenjidiqi.icu/gtijiliwfp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.c1oappe.top/gtldhntwat.html

[D26] 数组转字符串
来源：http://hz.xuetiantiany.cn/gtnbphrnbj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhongyouzk.top/gtccsgpxig.html

PHP:  implode(", ", $arr);
来源：http://hz.ywan-chungtsiang.top/gtffcxbabp.html

JS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtarbconuo.html

TS:   arr.join(", ")
来源：http://hz.xinyue.icu/gtfexotnjq.html

Java: String.join(", ", list)
来源：http://hz.ehwqpu.com/gtznssaecd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtxaxuzhib.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gtwtknqclj.html

C#:   string.Join(", ", list)
来源：http://hz.jqgufenzy.top/gtmaejvnsp.html

================================================================================
来源：http://hz.sufxvd.cn/gtlbmizrub.html

E. 字符串处理
来源：http://hz.chenlongwang.top/gtuaefjttv.html

================================================================================
来源：http://hz.guowangkeji.top/gtqyjfbrxi.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtzupkhnnf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtvelnhglu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtysddxphv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fzhhl.top/gtujgazifd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtehzwqtmk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guannengcc.top/gthffkrzho.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhixingplan.top/gtvbvzsakj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zycfv.cn/gtwbvusgsa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangdashe.top/gttfqnvcmc.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtwumrayfi.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gtirkexhwe.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gtukpztlxh.html

JS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtggqaeenn.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtcifohfjy.html

Java: "ab".repeat(3)
来源：http://hz.nwbrower.top/gtvixuvqok.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jlsjyb.cn/gtcpglvnmy.html

Ruby: "ab" * 3
来源：http://hz.ydjk.org.cn/gtpkwftofu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gaohongyu789.top/gteqyngbvw.html

[E03] 截取子串
来源：http://hz.smart0.xyz/gtigdoehsn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shuidangran.top/gtjeuluhyj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.316326.xyz/gtgsbhntwp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtkcrrgbfz.html

TS:   s.slice(1, 4)
来源：http://hz.c1oappe.top/gtodfcfklk.html

Java: s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtjzmhauiy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhixingplan.top/gtdrvxboed.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.52xcode.cn/gtidffibng.html

C#:   s.Substring(1, 3)
来源：http://hz.andypj.xyz/gtxozmutyj.html

[E04] 查找子串位置
来源：http://hz.yuanzhike.top/gtceadrfpl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fengsongda.top/gtgenucrya.html

PHP:  strpos($s, "x");
来源：http://hz.guowangkeji.top/gtywrectow.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gogol.net.cn/gtkymbpaoq.html

TS:   s.indexOf("x")
来源：http://hz.guannengcc.top/gttasnenqg.html

Java: s.indexOf("x")
来源：http://hz.birdmap.top/gtjvnppnqe.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gthztixvqs.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gtpuzfsnfq.html

C#:   s.IndexOf("x")
来源：http://hz.c1oappe.top/gtxosoootl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnxiangtu.top/gtyawmypiy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigfzy.top/gthlkzwcik.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinyuanbaomall.cn/gthryukuvj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtiswltzig.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sysykeji.top/gtwpzakhfa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zycfv.cn/gtsgwlkixn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guannengcc.top/gtpsbaxrhl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yangfankeji.com/gtcvbhavfz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.haohaochexian.top/gtdirwldlx.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtdiiiqvxf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj202588.top/gtxlznfgiy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgfzy.top/gtirtwrkll.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtyscjetcw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtlmdacsrv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtgoqsczik.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fzhhl.top/gtsicmidoj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.52xcode.cn/gtnjlhieqz.html

C#:   s.Replace("a", "b")
来源：http://hz.redwolf501.top/gtkuzawsxn.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtlbpavubt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258888.top/gtjbufvurs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zdqjudy.top/gtvhcvqnmb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gtafghkphp.html

TS:   s.split(",")
来源：http://hz.vqdsnc.cn/gtxfesksem.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhijiandao.cn/gttecmypln.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtczkddrsx.html

Ruby: s.split(",");  s.split
来源：http://hz.hammf.cn/gthvnztime.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxuanxn.top/gtghflzctc.html

[E08] 数组按分隔符合并
来源：http://hz.yueranfly.top/gtmdhlrkon.html

Py:   ",".join(items)
来源：http://hz.pycfn.com/gttmkikrqa.html

PHP:  implode(",", $items);
来源：http://hz.316326.xyz/gtdfozylmh.html

JS:   items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gteltdeztq.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gthzqxxayh.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gttjqzqncn.html

Go:   strings.Join(items, ",")
来源：http://hz.hywenlv.cn/gtsoyvjlxw.html

Ruby: items.join(",")
来源：http://hz.meibo888.top/gtaszjmcsd.html

C#:   string.Join(",", items)
来源：http://hz.0kj1m.cn/gtniaahlcd.html

[E09] 去除所有空白字符
来源：http://hz.svipenyu.cn/gtqpcdupin.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hammf.cn/gtshwuydkw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tanke756.top/gtwocrxezw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtznzcrqmd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtynnhouvd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtyeswwpci.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangtech.top/gtrvbucqiw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenjidiqi.icu/gtyshlsojs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gtiahzyjen.html

[E10] 左侧补零 / 定长填充
来源：http://hz.c1oappe.top/gtinfqvvzy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gtvpsqzuhb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.svipenyu.cn/gtdzjoudye.html

JS:   "7".padStart(3, "0")
来源：http://hz.jlsjyb.cn/gtfydwdbwz.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtjifqnvry.html

Java: String.format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtoabndytw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hywenlv.cn/gtkfqpheep.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtyocjbyib.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.andypj.xyz/gtrqtuxwxj.html

[E11] 反转字符串
来源：http://hz.jinqigfzy.top/gtfunruldm.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gteqlfbeps.html

PHP:  strrev($s);
来源：http://hz.svipenyu.cn/gtigdpykcf.html

JS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtxvbrdjnx.html

TS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtnjqhtztr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtpapfjkoy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnqzz.top/gtrujzsfwu.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtnpgqcvew.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtksofzbti.html

[E12] 统计某字符出现次数
来源：http://hz.andypj.xyz/gtxmvvwnvz.html

Py:   s.count("a")
来源：http://hz.sxryk.cn/gttzgmrwgj.html

PHP:  substr_count($s, "a");
来源：http://hz.0kj1m.cn/gtmpisufjd.html

JS:   s.split("a").length - 1
来源：http://hz.vqdsnc.cn/gtzczjmhap.html

TS:   s.split("a").length - 1
来源：http://hz.snrcjt.cn/gtptvuzfqx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtawhlamry.html

Go:   strings.Count(s, "a")
来源：http://hz.aizwys.cn/gtltfmpdpd.html

Ruby: s.count("a")
来源：http://hz.yueranfly.top/gtuoapciaj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yanxiufei.cn/gtdcqjobln.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtnhguqcml.html

Py:   for ch in s: print(ch)
来源：http://hz.shangyingyoupin.top/gtzbimxubi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtjbcyctrb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gthlnqzqfk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtqwflfeub.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhaomingkeji.xyz/gtpvxzhgkj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtdzfpmljt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtbencnosf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.316326.xyz/gtqeyawfrj.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gtruawkitc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtzjtwqpal.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shangyingyoupin.top/gtzpqdrupd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtrwvdiwtz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtilbisypx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ppjwa.cn/gtzsuzuxcs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.52xcode.cn/gtjxbxsynh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gtmguuejkc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtdwqjdvmv.html

[E15] HTML 转义 / 反转义
来源：http://hz.cucudq.cn/gtthpdbpbf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guannengcc.top/gtkmnicetn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cucudq.cn/gtmxpufwtx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.0kj1m.cn/gtbizunqkx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhaomingkeji.xyz/gtduvvxqgi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangtech.top/gthbatcljs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jlsjyb.cn/gtdprtjqtw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nwbrower.top/gthwrjhakx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gtxcbmwmoe.html

[E16] 数字千分位
来源：http://hz.guannengcc.top/gtqwktwmqq.html

Py:   f"{1234567:,}"
来源：http://hz.yuxming.cn/gtnmksjtbe.html

PHP:  number_format(1234567);
来源：http://hz.c1oappe.top/gtdbgaanrf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtfqfygcpe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtyfqxqrvu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtjtmmzwul.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtqenruafq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtlpbzlioy.html

C#:   1234567.ToString("N0")
来源：http://hz.tanke756.top/gtsfhoblyc.html

[E17] 首字母大写
来源：http://hz.zycfv.cn/gtnumvcnsl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yvedp.cn/gtmhittvoc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtgfaoadot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtcrvlyzpt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtkpvqdhmu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgufenzy.top/gttzwahwxz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuanzhike.top/gtbgpnakdn.html

Ruby: s.capitalize
来源：http://hz.sufxvd.cn/gtmxcdfglp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtwclmoosv.html

[E18] 模板占位符替换
来源：http://hz.ivvv.top/gtxmrhfxgt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xinyue.icu/gtbcuvzesf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gtedwndguk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtbvibhvry.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtritiwtpn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gtorhgcqcw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shangyingyoupin.top/gtroiuxljf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtnfcyvsga.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtoxnchaer.html

[E19] 多行文本按行拆分
来源：http://hz.gotoacloud.top/gtawwbpdfb.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtapnxfiqm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtuglkzoct.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gthycmagro.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtvwrpvyfd.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gtklvfagrx.html

Go:   strings.Split(s, "\n")
来源：http://hz.zdqjudy.top/gtwrpuatnk.html

Ruby: s.lines
来源：http://hz.shzxlz.cn/gtqseomqyf.html

C#:   s.Split('\n')
来源：http://hz.ydzc1.top/gtftmhnvtq.html

[E20] 判断字符串是否为空
来源：http://hz.pengpengdd.cyou/gtzsvodctr.html

Py:   if not s:
来源：http://hz.havefunace.top/gtqpsqncnb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.wangdashe.top/gtlqewfkox.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnqzz.top/gtbpeuavjr.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtbgdpimdb.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gthlbnyqoi.html

Go:   if s == "" {}
来源：http://hz.xziqi.cn/gtxfnffjle.html

Ruby: if s.empty?
来源：http://hz.xinyue.icu/gtjvanlfnf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.quarkkingdee.top/gtkrrffogn.html

[E21] 超长截断加省略号
来源：http://hz.yj20258888.top/gtiihwqsre.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shuidangran.top/gtcfdbhvnq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daxiang520.top/gtawwowpyk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtpnecmfqh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gthgpxroar.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtuhlkuiaj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtkgdrvcum.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtrfadbizq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtthfbfdpy.html

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gtfenpfhrm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jyoumei.cn/gtftpdsnzm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtfrihdjpg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtwbcnqkao.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtasmrxvvc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtfkiatspj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gtkblolhou.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtmjtiocyz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yongpay.top/gtjwxijawf.html

================================================================================
来源：http://hz.jlsjyb.cn/gttlbnrwuc.html

F. 文件与目录
来源：http://hz.jiagoushi.top/gtwikbduso.html

================================================================================
来源：http://hz.shuidangran.top/gtepforllt.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gtfzuwruvv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gogol.net.cn/gtmodwfbup.html

PHP:  file_get_contents("a.txt");
来源：http://hz.quarkkingdee.top/gtcioovwbh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yanxiufei.cn/gthxppdkra.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gtzthfylnb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtwhpvyfmp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jiagoushi.top/gtvelrilpq.html

Ruby: File.read("a.txt")
来源：http://hz.sufxvd.cn/gteuqfcyre.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.daria6918.cn/gthyxsgool.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtxiqsfsyg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.feifeiyinyue.top/gtnfhkrfnd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhengqikj.top/gtuzhayxwj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtuzihjcge.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtthcfepkw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtsfifvhkn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gzhubu.top/gtefbcyznx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pengpengdd.cyou/gtyarhzhao.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gogol.net.cn/gtevwcwvyo.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtryoditlj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tian-w.cn/gtnccnmxmp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.andypj.xyz/gtgjwmqpkk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtoxscsyue.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtjlxcahlr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.guannengcc.top/gtixluislm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinghuilouyu.cn/gtgezndewj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jiagoushi.top/gtfzlqwpav.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtkyxhcsid.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gtjmnlcvlv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.316326.xyz/gtwtongnbu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nwbrower.top/gtvzpntqhj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shangyingyoupin.top/gtpaxiebfi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gttlteqgtt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.andypj.xyz/gtuxxouwtn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gtcqdrtmxz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aizwys.cn/gtjfuwxyun.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.birdmap.top/gtsahbppfi.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuanzhike.top/gtwkxebjka.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gtebfzkdls.html

PHP:  file_exists("a.txt");
来源：http://hz.chenjidiqi.icu/gtlfjsfliy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtsnzwqmub.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtyamgqdtz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtilifooxw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtttsmtsby.html

Ruby: File.exist?("a.txt")
来源：http://hz.smart0.xyz/gtckflbckd.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtckaaqbux.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtqbjjsrtr.html

Py:   os.remove("a.txt")
来源：http://hz.haohaochexian.top/gtoaschdrq.html

PHP:  unlink("a.txt");
来源：http://hz.jqgfzy.top/gtevdvpcdv.html


<!-- 参考信息 -->