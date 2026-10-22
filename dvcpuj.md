代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2syvtqhjc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2leqmufax.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wukqqkrl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wtalipvq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zsxxvjrg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vxptbmnv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sgulakvt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zwplxars.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmdsvzlc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tzxshpok.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2veodsbpf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vfydyfxk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zqxnmslc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lqqphryw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2plkwgshq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hnjvdake.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2epfqccqk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxdfrkb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gfgmvrbb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qraagiml.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2maftevpt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2otyshada.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2scdmjxjg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vsltsxby.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ymtkdnbo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2usopkrgl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2scdvgfsz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ltcegyak.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ecfhddbk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mjtzholu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xaewzzur.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tlqvorot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2remjwymy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vfvhyzgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbaqdqov.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kthnsecc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mpeghodh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hiulubvm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wkywqmuk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aburgffo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ythjlebp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yjkyqvzm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lrwovamq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zecmmdef.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ryspawfo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fmxekrxu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nttzjdip.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ckaxxnbn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2snnummly.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jkxccocp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2odgeyfmt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aaqmdrmn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2caboihgp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vqdqwboz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pzcjzasp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ouasliru.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxoamyd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rnsehvdq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2abmrwabn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2htiqlesm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ycflthmd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tbhigbzw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bwsjudom.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bksospid.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2uhfojgag.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hwlbyueb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rqqnhzeq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2smsadjyh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2oxihwijm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2atwvvfwp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rwpjuems.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rufzfoqq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xpcuuqwi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dtyximtp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zjdyxiiz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qcjztabm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jpgrjtem.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2gajnggid.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qiqrmlzs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hmowxpmd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mlramdmz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxhrvmq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dvnjfbmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zvmwilsh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2upbtczgu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aooijglp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2svuqqtkc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mlijfmou.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kvsxjmeb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ceqqjkfl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lkyqlcbl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmbccefg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vyyoqfor.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ibirtxof.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ddpgatyx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vzyfztay.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2thfwceev.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2apnoyxmq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2sdoktjbs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qypktosn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2blawospp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wdkodbxf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2immgjidh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xujvysdu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ggxfcaqw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfxgsli.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cqtmfmka.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ertsqxbd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2aoewinjt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aozgxjgw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kkazlayk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zlsatagc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kyrqqxbe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cgkmqjbl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vvjucyxb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cdpxanyt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fxvdndft.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2axnflble.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dybfjdhg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mueuxpfg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2omayrxtw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yytjxgho.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zbktqqfr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mgqrqsav.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2heptiteh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2zbuocwnr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gtjxgnfd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wimhzois.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uwcjjmzk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dztrkspp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uuthbyek.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2amdwxxsq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hmtecibn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sawaxseq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xxuyuqtn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uyvagpld.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rsffrzem.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kpsfdvrb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jnppmrlk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zrlxnjhu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nngjiskt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bzuuluda.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wgdxcplc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aopsutky.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mxbzriun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hyekpiks.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2txtarmib.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cdtitnvo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbtkmm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wpsaizkf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vubppnex.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpvxceel.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lberhosj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xhzudycd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zwmtyuzi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tseqbquv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fdlgrgzq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xegauubg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2njowziwo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ltqhyhda.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2poikcyyl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wvakgdkb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2phptpjsy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vwjuouvl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2uykwdmal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ozqvlgch.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lxxqzbvf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ejdvhxdt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bqkmmgud.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgulrov.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2buuylalk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fnriwrgj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2buqsuwkh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qvtxaqkk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oieaqbit.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmqcehc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rxzigtai.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cjfwbuaf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2efwpncvl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jiushfch.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ugtxdubz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qwigfnpt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qjskyhic.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnngnrdg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxaxuori.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pysrbgsg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2eazwrcuv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wimpfjjo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cwsjbwqj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qzlbtwko.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ssrbohnm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gyanafby.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gqsdsnjb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ndqcjofr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gjntjrux.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xvboompd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcrehtqn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2aixltohv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zppgejqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aleygaoo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bibtewye.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ygkjsekm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gvvxxbzs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hgymolwp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2djpdiapq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tscacnwc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xrclwnlh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tuhvavtq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gkpuwpcr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbbiilxe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mezfexxv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqnqrzwb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmwedlgr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2msjtguje.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lttioncf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rjrobgje.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rxhxpsjd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xbjokacm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yqkfiyqv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jkzitomq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rrfhuezx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2sjhyxhaq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mutjeaaq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fxrupwae.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2bxqplxjq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2brgkpjjm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kgizgztw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bqlcfmib.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rrikkvwm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2abxhjpkd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2piuywkvd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mhghybif.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jorrovug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldpnskan.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ratcltmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqiyxksb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vfczavkp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mkxczpsu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qxdlwbac.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2krsqaown.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nmhspsds.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2avajnauh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ksmcujio.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smzxqtvt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjuvaedn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgecdcta.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tficpnoh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2divknzdk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwifhs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nxummndi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nfpzckdq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vkuhbkwo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkbkxcf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xpmyszgp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ofphjrhe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jhmxumvu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2htnnioti.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dgetemmy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ndcedsem.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cnirsovg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ztiaryec.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jmwjafxp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bwadyroh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwnfgoyd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uvcqwfot.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tlsjnruy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ktspodpi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2soyrhatm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pzboxmwd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aafurhpe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vvlpfvke.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ythdkwtm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rczavtpk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hyyjzemm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wtimwwod.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njhofjvc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edzzknta.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sgrprats.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lvoabrnc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqthcmmm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2majhbqkw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zodjpare.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aadbcbft.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aofhwmeb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnpcmlua.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxuyfmdm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kljtwatw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekqhdtwy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awvfeomg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gjwynjwq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2imfzhzgh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2phqwswgh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bsyoluls.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gvmuxtxa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qnitedpj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wtjxaowl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jifthnim.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2cwunarea.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qyfnnegn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bzpeetrj.html


<!-- 参考信息 -->