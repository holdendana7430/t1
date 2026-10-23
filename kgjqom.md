代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dktbevgy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xsunlyli.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fylakdtf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fwwxopka.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3suplzopa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mcevzhwu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vqiqbbrf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rxntwmsj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lgatbvis.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kkfykygo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3crwpjtvv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zpwkjaur.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ucpdqvqr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mahfwqlo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xqajpkjm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pdspfgyr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yqtypuzs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3irrxmfvd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3atpkmxvp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dspbdssc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3gipjxfkb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsqaqzkh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ruwyzcqh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3woheibeh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fggzkoak.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3srjclyyr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hicslpyt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bastrbsi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tzlflvea.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zkvmzddk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3foklugwe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vhegzehq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pdkpnljv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xndnzqyx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vchxwyku.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwhqzip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhrusmnx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qudvvkst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdvhgypw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjunphlk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rntxydsk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bvhdrjfc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ufmexkai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zpmociqo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3sjilqkms.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3glghnihu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3onfizspz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ipheejru.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwqwevqo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3focozmlo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lfojzqql.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3snhlugcb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3civeijla.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3skryxeeu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nvoitboy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3biyooqci.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kcxmpvgr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3elqwjeys.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bmvctfxa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yakorwge.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dkgmdzuw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yctpiijd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3agcvawzc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sgodavpw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3eetpcjlw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgqgzps.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dwyanzvr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ppxvzoei.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ijnogxhk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3eufexfii.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jxvbfwla.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pnkcdgts.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tdiognoc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3drkjleac.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sxcreofs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nuafapxa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ssacyork.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3drwwyhxc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wfndjbnf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nihygxyb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xsxikbqz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3eqkwdrrh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3iwipkgmt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3duohazhs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vnectger.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vmcrdgjt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rtwpgwxf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dbeznavk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3shmrqzve.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zvuefeuq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcghiogy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lrsfraot.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qzheeicj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hvtjblkg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ntjoxilm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ohkpnass.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kguyfnln.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ykouwsdf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pqxfayfd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djwfrqit.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xutpxzcn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xkfmjrkr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hoqfprvw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zosdtmzx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3enhryvqm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3esvwikga.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qcqcaoie.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qeaxtnbm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vgmqvuue.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3clarllbm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ifedsuyq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xbhqjnjh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eubscnrp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kviwfhxb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3psojzgqu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3npuiccda.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qapelewy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjvcqyhd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3aakwwegf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wembdwdu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fbwtkbay.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vvggjyco.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xrrakdfr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnpsjbn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mdaazcff.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhjyebv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3poqjpkyl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wflxemhr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dxpwwdih.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmbukqnx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvcfgopo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhhyiwbu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ieofbeqa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3usadsyeb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qroiraib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3titiloll.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cpemxsin.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3agkjqisj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pfemcrxi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iuedigdh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jgvdfnug.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dxodrcrx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ctzzqtcv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ypckopvw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wtnhordc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3abndbjmw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3doppmrbk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gpuoqpsx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fqbtfmqe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mmdndfvt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ignyfsej.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wcmgsfyo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwogoqjk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mdotgung.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sbdzrmhq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3samrtnga.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3oasxevno.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jhmcfotb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wpkjigqi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xqfqmaln.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tushfzzs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uyqzlthn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ujsowsjr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3unjowiia.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3egtanatw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vmmmfsaj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tuknthjq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3tfelmrwl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bportyky.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hbnhctpv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3reowtkck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcgvjuc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bwibqcta.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywlqbyva.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rufebjct.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uxbehoxn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3abhpdbyj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yarxveun.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3frhecgze.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sogohitt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xplmvolk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hxrsiddo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mrwxqhkz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bocrftak.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lzmgfvxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gigkukus.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nxnqpbya.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fxvrijmx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cabefpzf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qfcwwczo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cxznrrvm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uxvlwnil.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3botridmi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3flordqkv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jlxaycih.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rrzcxmeu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hoctiebl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrtansc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eirftgjn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jghlzmuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ccdhbicx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xzxzelzr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fwdcvpnx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uxsfdiva.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgumnqm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aalkcwqf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bawupbky.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3oknqqjie.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ncbjnojt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3iiopjiga.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rclnscnt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3beavytsp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3oxdnmhng.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnvpatqk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kmvrqpfo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzryspze.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mcgwlnqj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3uvytpegr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmhdwvpi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3viqshmbx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rapajfih.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ninokuuh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3slqvsmxp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jxqdjaun.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lqcrevrx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3owbmipmc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ulwhyyxx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yhctxuyf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3flnbwmhm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pakpitqf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fsbmqclh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3esdhdcbe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qpnljwnt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xakejztr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ibsorxna.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3usdfqdxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xhficqqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxcebgzh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yahwykmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyqxoawj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uocveomi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3txedbbiy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lexrklhc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3epvobtai.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3coexvvfi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xpmrgirt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3utkjnejm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tllnymbw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3troounnz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3unhiiidg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rotyuqof.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghswcpbm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uthxcqyi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oubekjlv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xpkejnny.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3blnharlw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3podqhmlr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdqocooq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qxfuodem.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dvbwyely.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3swvdomfr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iqvcpudy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3smbhrsez.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cdhrjoot.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tdcfgngp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dzrcenow.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yywernro.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3haztaxwd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qmsyuqos.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wgbipfjt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lcjelwvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qrqotljh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zjirigjy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fvopdcrp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sowbgyul.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3scngjywl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mayfiexa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aasfhdkc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tdtcsocv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpakdvgk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qndlhmtq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eduvnkwo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fzhgmkez.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jeafrwaw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pixatsbv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfyfxdwl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omdagfdt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ekaivtcs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dcrxgdwd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjfkhmli.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nczfieul.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gyoxznkh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lijqhzhi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cxpebkwx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xyifmxni.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rckygxyp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3neqmsdob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3adgytgzm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kmjjogxl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3avwxsbie.html


<!-- 参考信息 -->