代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rufchgjf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fidhksde.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hboracsg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lxudnrjb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wksjlrdr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lxgdwnet.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xxvwvxgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tjvuwryt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fbzcolzm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mbkstvhi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rvxdgxmp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lixljxgz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tadhdrcq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3suqtvayo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3aesudqoq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjodzfxf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3utccaybm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qmbqjzul.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3robvcxll.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zydtlrbu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oadaxphd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olxpbnvc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vfjmvtsx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zzuksvqx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ltzyausv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pootmezu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sntwnsnh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uxwicrbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xevofufg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3quaadcpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieraepdm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3oenookxi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lbegpbtc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fnirypcm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kotrshvb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3skeljyof.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3mncmgjus.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjzdupzd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ffkdxrip.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3trstqflz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ocedzsxm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ofohnmgd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3esfxofhy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mwsegglt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3znfldyrh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwrgcab.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxctpktr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3neppmbwj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bpktewjq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rwqurmxj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nggtsfvm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jhlbhxdh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iytxaszr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zyxupkbm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqcwvbs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uteffbwc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3sblxyxhq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3lxffdzud.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lbjsznnl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ljvwvhog.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mngahadz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gmielgey.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pftspipf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3quwwpbnm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3caqgomdu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3johcjmal.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hsmvvjgl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bdisafoj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dggfcppf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jkbiiipe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gjuquhok.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wrmsxdov.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xobxpivc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jsujhswz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3drlykvsz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tprunhfx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3armhutew.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3orzgkrio.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmqtdldz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ubcrqrns.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3slxpozks.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3acudqpyn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtgayhw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ypscfzok.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kllwvbhj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ohsaiglu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yedvrnkq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3azwxurev.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wnltmrfc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dqtiflac.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pogxsgtm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vksvrqbk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ojqrlhgx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fuuolnnn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dxsxvhml.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ftkpdqqu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mwusimhf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mdzfstwm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lmczaggb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dzooztuv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hszrphtu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mnhzkifd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jlxuftpq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dqymioxo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkfaffkk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ymlseiip.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hrqdidkl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vqzokrhn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zdovkjrp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hintqhzk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3oefkadoh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cxvwdkda.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cfbwvnvg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nizepunq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nihtmhrm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jcrwywtd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mkylmwku.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tunjsagy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vdumyqzv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3upjyrrfj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3uxgioqux.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vjntvukz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vtlkllkr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3heddeoen.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sovzovan.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lmgcemyx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pnnlxbca.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vokbckbh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aschalsg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zwthktvh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dxesqgva.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wrwxxkqu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3whbntumy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nvtvxtpo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vqqdnhvv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3egmbodhn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gwajjomk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pxyllokj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3whshovkb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3esdsqtcd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wjjdbnok.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mljkshvd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hiotkzje.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnllkcop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nylnyunt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3exhnmflb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zplhwzao.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjewllnr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3efvxneyk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ojhisjma.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zevpqate.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ohxttpue.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yettqvrb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wepwhtdj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fjplgeou.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mezvuewf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmwjilv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3alozypxh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yckfnlfd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovvlwism.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdshivi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yysdrset.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3paerppai.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wozjmwog.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojentlnu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3skilewtq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gdgsxedq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fsohupgr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gpvoicev.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iloevzqs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3seqihkgy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ixiuugrp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hiawgarw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xrtmwuzt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3anhsamsm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fjusrvso.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3edvljpqx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pcctkyvd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rncjtbxx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cgzmvnnj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsubpqsg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ikujdvos.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ekmfwesj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3toaslrze.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3spelzjsr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dankuvwk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kucaiwnh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ligdeuyg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbhplco.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3okqmvhjf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3luuyklna.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3nfprlkjc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zyjcodha.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vnqnukts.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3whnslrsm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3suwkbhii.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqwrppxd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lpbaccjq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3khhpzjrj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bvbvuaqf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zwecljas.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pouqicyy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mjmxxbmr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jviujxzj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lwueetga.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3onqrpsfr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzzedqcg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbaxpzhb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yalpwgwh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3iwfymerl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umcyxznd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dayvmoef.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nrzbjvsm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bgnexxcd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cnpufvdz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eieohzeb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ddseiviu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dalbczmb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qovdovas.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xuwzoyiq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bdesrbhq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmhuyibh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zuaxpjtv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dlrqvgpz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tzzoovot.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lioyoval.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3oqgldzfy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pbdlgegb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jgfecsnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqiphuau.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bzztfogc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irkgbazk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kuaepgsg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ljukymla.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnrkmfrq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3elgijdaf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wtwczqyj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkcpucxl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3doihhcyk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfnyhlzr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3brbwqvgu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gflguccg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3iniiszwf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iwhcpjkj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wicetprq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqemvdpo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qfhkzids.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gnifpizp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lreqzwoq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3npgxwadb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kvclmutq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ropwwqvo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ajombzum.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aumbwfql.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pcthnuzj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hvcfezhz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lemnmmmm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gygqfnai.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zjeqgwbb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxipafwv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3stgfewyq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3knnpovfy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rgdfzlbu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sjdhigqk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3chapmeiv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yzmwsque.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ccomoomx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vnplgxyb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ualsilzf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fcetlbmf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ltejixyz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzpcnpzt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxpiskat.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uleodkkc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmmffrt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txitbhda.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnlnshlb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pbmjdcoa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uymvhyhd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmrasbwb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egcumjnb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3waejwuem.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yfiwnckc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrzpvnpt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eoegljjm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ukngxcww.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3obxhxycy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3omfzwquk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xhqeypql.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3auuvvlrj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lqyffsfm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ypnmhcfs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3yrhmtnfx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3umejxfih.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ahswzvhb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ovqhdqpz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ndmqpbzv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3msuityzr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fegqeunz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kmornlla.html


<!-- 参考信息 -->