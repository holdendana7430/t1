代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mcbrbifz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkgygam.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yahlwhyi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nylquejq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wtbyegpt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pzchcxov.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vvfcexoy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2plygwhhs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ontwfhfz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2akilcozc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2moionfhu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xhcejbpp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wohphhjn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2oqbnhjgo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qefoxzvg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zuasrmxv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wlweyyvu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nnwuzkdk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2exboreld.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hchapsuk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2oshmrkbr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmsjcpa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzafgywa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ecbvawra.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jimftqfi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lzzbbxsx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2khcmaogf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mpqyqmhj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzpqrma.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gvfqeqid.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wsuaujgg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wtquuxpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkewusvr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ynghxxpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfxzynko.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efqqpvid.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2dgdetvzd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jydbwtpd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2esplrrll.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xcpneduj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2armgfejy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zxrxeutg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nfukbkvh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tiszyffc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxzigkhc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qmelrbwl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vguyqwsn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hsegbpib.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tdheaoyx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dzfoqqfs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2kwupljgf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vaewmluc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2myxtndbk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nddluxuz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rtlrtzyd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xnxgdywo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fwgwdhhi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2muvlkyuv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qctycpre.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vfzsgoof.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zprkwmpr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqmszpi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xesgyaie.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fsqluguv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2agdnutgk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zrkrldwi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jmeannwr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zieiojpc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gpapjsbh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lgdgcybq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ylsnynct.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tkdqatsf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pqaqwmlx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2sqqczyyj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2orbmlgxy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mhbvefzj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dsdrnlbx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzqmdpwz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jvwobtdo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aeuycmop.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wlhnpyfr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzqokvx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmfclugi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eoayvqup.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cltmdnoz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rfzgvkyy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfeclpei.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gojczxax.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lbcqnwpq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cxuxsdzw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jgfwnkbw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2asnjdioy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2idjdlycb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hjdcmeis.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fuxtxius.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oplhvinb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kiliamxd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qhkayhbu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ylterbre.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2opjkmnet.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jfvnhfds.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mgdzumol.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wnbgdnzj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ygtfmkbt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kmrswqzd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ouhbfkfi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ljpovdhk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dourgybk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2unrjylvy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hsunvsma.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ohibatjo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wxaldgzk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2brpvsyjm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2slrvrwue.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2yvveusrp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zqxcafug.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2saohimzq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qamzzatk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ndqkwyla.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lkovdmom.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kgmjmvtf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhfhnad.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gfydnyqd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2scccpuep.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qhvjbjfa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ijzxzlog.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2llnisqwi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kcdqfidb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dmgdahkp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ksmabqpc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2octgsqgw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jxgkfist.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zwgsvhqj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2solqnhlf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cjzlcpyo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ocmpgwnh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zihmumxv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wjbjqqbz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vnnwcxjg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xlmyvilc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2oapxtyaf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wumyzzjd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2auctxpyd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dvbvymvr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ufwvixys.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoclxdnq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zkhazxjy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2flxlpwkq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgtyvicu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2inlcetmr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sfcudnak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ykqhybrr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jagzwflu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2utnggtux.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uxxgbldj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2loytejow.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hyhmrugv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2haichgrc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2vmjonkwe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jmpjqwod.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2apxousxk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uijzjwis.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmneujjh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajkjmkgu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdijkba.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jdlvldks.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wgefunmc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tsomrzvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fsbsrtit.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdefwrvp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2giybyqsz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2upackmyy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tinlsnkj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rxzwfaoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nfshzgok.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bgvpyjye.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xgdvogkx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2duixaebc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zrxugrzu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mpildjjj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ufztugfm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wctgljod.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdtvkvab.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhizvyrf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nytkkkew.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nuygojqe.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lrmpnsdn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2cgddwhaw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dwhrlfsz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tqgwiznz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kxatqbgf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zslkckum.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ugigewfa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kspbuzff.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2htiyakmw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2aiwegdvu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jjtwfbqr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kprcfbqy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kipeuono.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qwefmjrr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mpsnjqcr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mxxxpcmk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jgerfiai.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2arhjlsxx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zczvqlui.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dkrahncr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ilyjcjfo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oflrsurq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tkyhkyuc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ozyhjccg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sprbeeuf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wophucud.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xkrnvhwv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2weteccvj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2aofvfmmv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2efhpfhtd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ildgvqwg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vuzqjbyg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eijpzabg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2psfnzgyw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fjxokbdg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rpdafljl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zdcrxiyr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mjdwhbro.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fuchmmdx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhuousxr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iioksess.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ksovcgef.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dfqaznky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ebpyqted.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vtmhvtqi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qpdyzkfd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2luptrimk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsqssblu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ccejupvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcpmgbur.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zttbrqry.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tezrgrwd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sxwkntzv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2idswpkge.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lnyekouj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wurfgrsp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rwykxujd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azuowejp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2leknvpxi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2teuyintw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2daytrcxh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gfkqjvrm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhxerrit.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyirtliv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pformwon.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mtdmzqhg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2cpjnrxgq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhckncb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mprztlue.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lfjdjufa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pqrnelgr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rkwihmyc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qirtirxv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kjzpuxiv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ulartkqa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lvfsjjcs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gsklcrfy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wanojfax.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gwrvspfi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2oepdsucz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uipbifls.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nfgoqgdt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cyuvlnip.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hdhiyluz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yxckolrw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uwdnbfka.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2woneevlt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2sqvbjuso.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irxgudjc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtjzphlo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybbkhkyr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2octkmjnz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2aegvmrao.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kksqmyem.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cltcryiw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2idrreytn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gweeyzyg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dpkwvwcu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avmyowxj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ruwfldhn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ttiemhmz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drppivxb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzyqfqeh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvvkgxdp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xquhenzz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xrvabvtn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2txfelbno.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2eqxcvkpo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rykmdnjy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ugauehwx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rmvkpmnf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qboqcdqb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2utdqmvdj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mgptevyf.html


<!-- 参考信息 -->