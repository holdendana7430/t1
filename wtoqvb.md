代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlsgpfqh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ikgzdcez.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vvunrjfz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dmylvsgj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kkgsukkn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fxglsduv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gydapkrb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3grjdgzkj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbnmrhu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3belkbjtn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jczwtezq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3sdwmehxz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3whoedkvv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xobcfbgs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vtwubzjt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3meaqzghx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zawhtcza.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsdmvxve.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjthqo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhntrmpb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sgxgqlof.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytwtrpsv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3puoqlhqv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pisfzrdn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fyxgyybv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zejjjvax.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hakuyyjc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oeixlchn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pgzmmqgx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3axxslcow.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hpydwqpd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fxphugdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3achlyyus.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nzhjlpdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkuowrjm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hzpietui.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vuqzcyaq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3doqarmly.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hcyoaqqg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tutzhgcs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ynzrnwwy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bpwrpinz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bmqozzlh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xmjzmggr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlhxqela.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dhzgyfab.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aluralcc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqiowuuq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3txcublds.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsodmzd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qpglrwzm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mitmkkxo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tcegnxsj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jgvwruzr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cbivmvou.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ismiflht.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uypwdunw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bfebuxva.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mzibrnxx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3czyzpymx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3synershj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3sdwfanml.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nejwesww.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3orlerbom.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dzihauky.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vqltuaqj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zgtcrbld.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jdsutoos.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yawgcofk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bkauwawz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lmoakhie.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yfvulkhy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nnorjiht.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3csucrizf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fjzeqgei.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gvkhrasx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3syjblrzq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cgzvcfmx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zycdcsty.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qoilceel.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3keozljga.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ztbgqmzk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rkwzdsym.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3srxnrbfu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vmhuumig.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uzpzittj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nrttmjfp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nwlvilji.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yiwpohdn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wlabbopf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xlmzyzdx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhplacah.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ffiwzizw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tlvtxqbm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qmhhdtyg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3idoferov.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mqnjrouk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xeshnlbr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ezmpklcf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dusyhbgt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uknzfmvs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bjwjjarm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ugzdfwmv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rexcufju.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jhgeuxsi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3glvcvwes.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ghreuaht.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vxbhbsfh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nndticoh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fcfsptqd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ncifbbva.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3axsmystp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bbfagrou.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qeceduby.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3opliosiu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xjdgplhk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ppkdwhtr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hhjpudte.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3phubdvdq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cwnusppb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3stgxxzjs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlalwlv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nvtzgrpb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3furqjjiq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3yrnltawf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqftatbg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lhobxkha.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wsczrvfs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ixjwnwki.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3voqpapjh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vfdusdbc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3syzytiuo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ssndnwwm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lvqyswtt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lliyuwru.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vxzwhfoh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wfdepsnx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nfuintqg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahtldtdo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3efvmuijc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nnowxndr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ighwwhds.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3mwhreywa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vgcjwzlc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pkwlkzrb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvevdrjk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ghijvqus.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymxmfloa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xwguvsir.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pcjwdelf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yfgwcunb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lztddmog.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jfrnmcgf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3twubbgzb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jinuwpzo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3olwuvabz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xaukpqbw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mmdtlxch.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mljlhwlx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ouoyindx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vzrqtpta.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3belbllqk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zspfhvqs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qmhjnxcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zawtnygs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kddcnafd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3elcqzphb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgteosdl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rctbyszk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gvodacos.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pyuescfl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3itterbzs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tgkotsup.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dsrsddti.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xtadvkud.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vmyfshdi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sgzmgmtc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jggyynuk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3sjnsccxt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3arlniipi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3phjubkcd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3djcfswwh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uavvsvoa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sghvqcxf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdgqzss.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3akanwetn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qkwyipfg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xjjfnlzw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ptxxtonl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3djasgxqn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3krnlanmt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kabmoqpm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rtmhxrld.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nmrspoeg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ptlmggic.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jwxtzwjj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pznylbvw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lticxnut.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zkhyvcpm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fodlvmen.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cbgdoqzy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qpuivhdf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3knpmgucn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3opsyhwsh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yvkyzobp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wtjiwgmt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ovuwjsvb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3djvahjnf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gtmblsup.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgumjrae.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3eovcsqfh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lvzwoyyy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gkbqytul.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lwilsuxj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qceybhrh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3dwdapana.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bztgcvxl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bonvuwgj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3deicalib.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3faaevdzb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fhgdwjmu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cnfabfbz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ebsbtfzg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ginfhxlw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xqdrnhxq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewskohkf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ihoncutj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wuatirkv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3afnhygsa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3umwzyaiy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wnsdjaih.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ikduinpm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pzixcsmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqxusdsi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3crpbsxpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avqoseww.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncbnsvib.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3maasevew.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3obilbcgv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3asgixosk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hwavgeyi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3anyqbkhi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3arzdymli.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuewsjso.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iauuhrwx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rocpzcrn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eablvzuw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdmqzkdh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gchgteti.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3flrsavco.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ykzxoorc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytuvfyed.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gaocnhzx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbupiqbb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3iutljwyb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qkkxsmbl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3krboorwb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eabwpiaz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bwbjbkoc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ytsdqtqr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kcadwjye.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pakqmgrp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gbtjrkdj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zqdbjbad.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mopwbfbw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3etjceeri.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gifhxwip.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jwsiwpkg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ljanmaso.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wdxsqxwz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3popmviqj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ukauqvzv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3quudfxdl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cpxqzkyq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3igyxbnin.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dcslqcwt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iayxqodd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ehuynepq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ljvjuosd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qazfabha.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnumnkhv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3whxaosmd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggzuhwqz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hngwxtqu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdjrizha.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhspmpqs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jdspujih.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbfryqdg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqjshifi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mcdudpfs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xhusgmth.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qiyxdnvg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kwevnzrt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yefxnbuu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jcskqeuc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fjxyeqoo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lzrxvxtu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tckilpmf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lcjrsouq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3igjbsryr.html


<!-- 参考信息 -->