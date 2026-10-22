代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fdewnimi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyynczo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dhgydcbd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xtkvtert.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xsjwlihc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jqxhjbsk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lpnaufsg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ajyephrc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhnwcyo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wbhchvyv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qehjwfyn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2iasxjlpk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sjakdwsx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ejwqdvzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zxuclvww.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2dupxvxor.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rcljazlq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ppcmkogn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2enbqarsc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2krsnhgty.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mrzmkkey.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cofkrrof.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2aojaujca.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2higyeytq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fcjtlkne.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cijznsax.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohfgolvc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmbvagsm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qjnprupl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpjilron.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wcugxavl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xxrbrigt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fwljqate.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2kupejvce.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pumhrqhc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fysxlrxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trwoufvp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2oogcmnbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqfmhfxd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2abqqmfjq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pkaniuua.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qcglscac.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ucutgaub.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hgechgfu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mjpwkubq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2liahheby.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2foiwsyfn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bmhwxxue.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jyzfxygx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eomigkao.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2olzzcqew.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2txxmxrtl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vbafnlzh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tfrjlzco.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lklmzvza.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2higvlfix.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wqzojndp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rwiwzqlk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dfxtmjvo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yfjxlook.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uizpywju.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kbdorsnv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mrxxrrjs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vhqfcjrb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rxgjgmuv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hxbaoiiy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rmqroero.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xdqolfva.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2peghedut.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tllpdsgt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jpgksozo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dsdqbayk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ozjnbqlt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pfjvtrug.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hcvkqmsh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2orxoncgu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ljvcrehw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jznhicul.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2valvalmh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jpougvxb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2obrpilti.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vppdnivr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iiiireia.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ghchnajd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2errhtyhk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nykhidrj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qmrvwobg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2chkeaboy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bgykldvk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nghihnfo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilbxycoq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikpyobox.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2veptfvpf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zwoafbum.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2etejzdbb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwnvahrl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lofzdbyt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mlsexqms.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fygwgqkh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oirppnvj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pmjdekvs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gcmazlee.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pcmewfzk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wlolroih.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zikihtqc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nundwtin.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uhyhltrf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2asamdnxk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yqctizue.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tngqknde.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gxonxnmh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tszugpsw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wsyxnszq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2efrchziz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jpnickte.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bgkpbylt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pyfgomdh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qwiltaky.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kvtlpytc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2apjiocxv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pduepwcl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zvosvolv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wmvcngwc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vlysgkrn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rarlwzvv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ssknlaly.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2blwvakxw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2crocyplp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ivqcqdkn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ykfmixiu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uieeitaz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fclfoinn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tttpzfmz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mxsniahz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zpxeqopk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ltznjxby.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rdmadful.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bzmltspu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vafitgdm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ldyjobpv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kkmepfxx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mugrdjar.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfuzofku.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qjmefuhs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pwtztcys.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oecjilse.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2oeqiwlth.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2beuvgtgw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qdatwykc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaogjtfg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2avvbgida.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpevcuh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2twmpyvlp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2povwujii.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2elqickay.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocsibdfd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2skevjdxf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vecadgae.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yfhbjiyv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2awsuqmzx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jbuzgaex.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zaryxtdm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2yhexqazu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hrsbnacw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cvoupnpv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bkebldpf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qtgwukwv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjpstpoz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hqnfzhdn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hnfmfomx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ggukvxtl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgvcsios.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cipizavw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbdnachn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qfbsjmpp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dzfamuvn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jncxpdxe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xersxedh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ujgtkpgy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jkdudnzk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tgnsheqc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kneogtww.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mdddyucy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jtgwwwng.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rznbmist.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2inlvyeoe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yagukcve.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynaskjyt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wdhcyizn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jszzcyyk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2arvchlxf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gtodkmut.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hetsdvrs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qjomvxmk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2taerwoco.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2awypahkl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rbvimsib.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qjmunbgr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kpqeczjc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ttsplrpm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ogesvxmp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2htsdivpq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rehwvnyp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cflrvamx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qukpqyes.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sxlbldje.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fhxuluvt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tehhntui.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kxtwekvl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tiootgmz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nyrcqiva.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2eaaftlgi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cvwxkitz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wmjrwbkh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cnzvimms.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oaxkrweu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lxsvehrb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yggwsunp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kztsdxxu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bpmyvfvn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2oxuydglq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ahcfvfsl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oqobiaxb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ivkfrnkt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gpjvrsvz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rsyrvvph.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mziybaui.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dcjdudgm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2upplopsz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dvnfpgla.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2defdeeqc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bpqqaxby.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hxlxbkpk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lmpkadjw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rgywzrhe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wavwkgfu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2slwhryic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrhawxam.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wwnpzutb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjfyrwqv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrvlkbwc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kolfqfsx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpsspuoi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2foocwner.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wsmjolfb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mbusnhdf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rhguqhbs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwcrujdu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jbaqaogc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gdeuhuyn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kzhhymtr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2neqfqvkz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmsraukr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ljbzbjww.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pqnfqwli.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lubszstq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gpptptsd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhoddwmr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2uelkxvvw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rprqqsby.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dpicvomq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2egqwqxpw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2luhyoarp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cyaozlsh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zjkddsyr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xkexinjl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qaiahjrg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2suajxxon.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bhhojymp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hatjhlbi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ypsnraye.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xwtsyfmt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kalomiby.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ryzvevcy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vviafsnk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rhsllogl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kwazneha.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2npipvfcq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lilreguu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlajzkce.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwujthsq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sozlufyp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2waqcyvqm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojlzrlxy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydjubhgd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jsipddnr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhcikpgv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvekmmrn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uffqxotq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2brgwurib.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zcbrqtle.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vnbvtnyv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ouvketff.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2raphqibm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rzmzjqgi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ttrlxnzo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cvtluxnp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jmarlchb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yoaxxazs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqgzmnvx.html


<!-- 参考信息 -->