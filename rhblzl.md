代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fgolichy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hifjksba.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xqoamsvu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zrtuqjlf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xxhcjsaa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aphbskda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dxdevoxx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xjwcpcbx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fcrqxzvo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cvqtlnsx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rdqnohzk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lfavphnm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bolivpqe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pwxbmsmz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ivkziqir.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cqsckmil.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hxgfmkgz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2plwrbofc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rxzflxdq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wmlzycaf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hphjybny.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cepizoww.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hweqpxmf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rzmdgtzr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dtcnlyxx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lkcqxjxr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yjtuirjy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iyhkexzc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gbupttep.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nptyhnvk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2blkztaxf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zfkteofh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fvzppeuu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tpmzqqub.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mvzkdhzn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oorohcyi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wdbzfmce.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mcfkkwbt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aupqfwsf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mvaljdfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwwsywod.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2trvpfgzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysdzlnww.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pmnbgdeh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eqwzpiyp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2adyqgmqv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ymqnwukg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yboyphko.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ypybgfjf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2excxhxvf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kdaiwqsj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rbtutxff.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zfprkglf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ganjaptt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zxkbytyl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2snbdggsf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pztcbqmz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvnrssp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrtqbduh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vupygztp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rucyhfvw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wbkqoqzt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ofptqhsk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lihpnvva.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2clwkeowb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fzwyvrdd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2clvkqxgx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yvgiknsd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hdmnrwbi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ymadxnjm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2szytizet.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bzjtqfts.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jbshvsuf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzatoky.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iedtdxsn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rcbpqyvu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bnxuolus.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nrqsncub.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hpejotbv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2itkjlzlf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ncxxzojg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pxiaaqqb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nfvvxags.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mggxaqnt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zpxblmig.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jgrogyqc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aukscqdh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wdvkxmyy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ulgyuxut.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bljyghjk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kkrxdrxi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kwdrpyaj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qdihfjjf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2omnheymc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ibwslzdu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2duwbokqm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gmwlohgc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mildohcb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qnetdzqz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2klolwvcv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbhlbglj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwatzhkp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ssxhnzws.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xzenxqfa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2elfpggyn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vyevwzbf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jttwiboh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sijujzgx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2apgkxhez.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bzmcenje.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ixxhvdbj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ozbttese.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2snpgoqaf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aqeyioqk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nbqerjvy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xbbglbrc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2oamwdxdx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bisdwllm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jmherhmm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nwfvncxm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2looxhnsa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zhxmlepa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sunhnjhy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xfjhmgsk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2reeaayui.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fipuivsc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qmohzxvv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wllakfgj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2twwmeawf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rkuurxgd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kfyyyzsf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2axtancaq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pnennsnn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fuplrmbc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2picytjvp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mznuyosm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rdkemyql.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2znygboom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xlaiyflv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hxvbelrx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yxpzmxpn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2adgwzasm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2erlwxdra.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bkboyuws.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wvoxqjmj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rkuztlmx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tuwsmbba.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ybchkiuh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ggxoloji.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2weapdgbe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ptyodmnr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tbapxern.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tkpyyuuv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rysdpwbt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bizaanfl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iqvazmjo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2atiauzfu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aiocjiio.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jvetszdf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qvvulvjh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hephlcbv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rkuyupip.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2uqvrgxof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2monywbhv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mvmdfztc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mxeqzcmn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2eyoshqwo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vigcuwdu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yfuvrxum.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eknldaxq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqnzcuy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xwbdimli.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bdfjgjir.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2istybqtd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ahtddtqz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crnpevjy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhhvjjtt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tworhqbh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uuutolap.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uturjilj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mlfvxmur.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2szyckpjf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2htricqtv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dsgsmkul.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rdxguroi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2avbcbuqn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dfbazkbk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iocxkdjs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fjvuidws.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pvrjwjll.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ugcnhxfl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tfxoyile.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cjdlumaq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rsgagooi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rfxfzhfo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ldbrlaid.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lbhhvajs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2upacjibv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2thgdnvcd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dugzemnp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bdaxxlhl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lruhegdn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ercpbgby.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2twlftypn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrczifmi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tcvyyuig.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rpfabtao.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qxdoiore.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vmiatxta.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dxjbdjwb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vgjzrned.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tkjlulej.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2craeexky.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gulwhggr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tkhzyaib.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dgjmltgf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dcixsqqi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tckpdlmm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lcvhhnrp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tqpenffj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2nfbxittr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2juksnycl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmpxqubl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uziysqln.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2szaagbew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gkkeyhzr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hgfkbbab.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eheahjnp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2buswwsds.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vbqnjsxj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pozbyrqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hlouqswf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ollljynp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cacemlsm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2volxkfgi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gqjoiuuf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xiwjhatp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mybwzswp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2odlqjyux.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jyruslqm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2etvqjdsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjpxghae.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fzouyczw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvlmefxz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzxxgoak.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cljvlbkv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lrwbymmw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hendrsjd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dxwmandf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xnuxbfyj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qikphpya.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmtrdwsr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lrtvslzc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wfdhottu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2npmwaxsz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtorrhld.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dllyiuzz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqoealrn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hxebbyrt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sagmgyna.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqlbiyi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkzwtoke.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qgcfleug.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ualpirdx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hmfstxxk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2upfdbkbi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gaiostyg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wcphzlpd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tphpxzba.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kyiqfhtu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jimxgmzl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdyqumbr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fgmlqyyb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bachhniz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zvdwvfet.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ppuumika.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2leqewpmm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hzjtqnxe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nntkjhec.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wwrmprvz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wvglylpg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vfhnipmh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pgyghxbx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eyjvkmxx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkoolfbl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tsvspghl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ixcyozzi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aiuitlyv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbvjfjbs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nieroyyk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2suvwngox.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wnaoxzlh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgbkfdlq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjzdjynf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2huadrpdr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdetncvu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzsmzjkp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mypfzund.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kzuocxvu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsbxxur.html


<!-- 参考信息 -->