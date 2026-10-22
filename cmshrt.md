代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2trfnqtpk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ypfpslpx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohpkpjom.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xaolpkeh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjazgri.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vsbhclqu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ievddcwl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rpvubbew.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxprfceh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mfebgliz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rguqtpgw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2dyvhyybw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nppcnffj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2egwmjwcx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yfgbvpzk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ycfqvbhs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mmoiywbs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mslnnjzb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vzehgwdd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bayofoxd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cvquukuu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fiovxuin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vkygzpnj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igiqvkde.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rwrklvyn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wicronbk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zmrsqkih.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uikxscod.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2emmtrddg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pjwvkojj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gyfjwfur.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dnuyooln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcqpqzxc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tqfylbcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvihytzt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvpdqsuj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qtlyizmb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wdzdfdgj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2owgiitfp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vlphdfax.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yswcggkp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nbgzcrgm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hlnlhlcl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iokudoso.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rytwuszv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ciyssyac.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zubxdoyp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tosbftpo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnfvfqd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jihnifzu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvrsvzpa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2glenkxtc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bjikcekc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2twzeaqcq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kksypini.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mefrxllu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kxslnqaf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vowuqaee.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lrntsmaq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rpeahzpx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qzolzcov.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzonpap.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mitrrysl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cussikro.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xmsxofdu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hpfcgtdh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mhwwdaup.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2abixytmq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dvhwjddg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sdbbpbod.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yzmztavg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2liuegaec.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iujfcmrx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2peqxiept.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hgwjgtcm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pccuoljj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zheblzqa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vklsanoj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2uidcyppq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xonmbxuy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vkveggos.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uinvdmet.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmxobepu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vxutafrx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mtyxfjhi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ddcwigsl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gttklkih.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qdmevwqh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sizwrrie.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xjfcxizx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rojekqig.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ewssvlvw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ndzxjkfn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lixbaime.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ujyhmtmo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2unzuziqf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gqqwuzkz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2brprmzcr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kwjfkdef.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bnrojdlt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lmwomiaf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ymgqhrne.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uckfybll.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zovqrber.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cawtjdwu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2krloowrf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oyxxvpxr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ebshjydt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrslpwlw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swebntno.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sqbmyqim.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jydsuxgz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2obwfippq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jopdvtry.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cqufbpgc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tdshzeni.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uybsszhz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dkywlnep.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xazacsjq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ibzuyuju.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oepsnfhm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wfnlswig.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ebmubiiu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sirgmqsg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2sykpxpge.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rwuszuob.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mbetsnii.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2igprsvis.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qowdvncg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aydnsnzh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lxeztcun.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wcrzerhv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xcjauevj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eybapttu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gaptfyvs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pizrotwr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vnjbudkh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vvklwnyc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2aybcwlkb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dzogptow.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rvnumzgd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gjvvvycz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2renuwnjr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dpqyical.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjkncyd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmudwybk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hagcizds.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwgyoyju.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2btcgxesp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ypsunstk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gbjgnmaz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hbohjzbq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tsxafhhu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nfxkbshy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kwyzbibn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fawqshve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfqfmdsi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbixrwq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kwjosdoe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jaoabuvv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tzubbrya.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rcbyaepa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcbgfgg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ddjfpckk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdpfcqy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2scvvpxbr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kahjtvkq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkfsdcf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wowfenrb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndlrbydx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2exssgkie.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cjfoogcp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ungnufos.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nwsyxltv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dtujgowa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ejhqlqbn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ggaelufn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2hhsuiasc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fyfinnbc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2avqhksdk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2usjhagxb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fafdcyuz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ssjwcugx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ajaxuxuu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrmhcwr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gakgautk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2numahugf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wzuhqjfw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ldgjyckt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gabziqmb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gakhxfeb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2spqtfbqg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2akcswukd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xysvqwkn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcikned.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tydttbke.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mufxlfvk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2liqcgqjf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nweymjed.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qorunikf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gmqfncux.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xdnglukt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2usibibgo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hufamlxb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yatnihzj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vibtmtla.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qlakvdck.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rqadhshh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2buxepwzo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvvsyaum.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkpdagxv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mgzhswma.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ksvcithd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wvuvjnmz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wvnkfjdw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mtedexjf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2asruhwex.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oviefjmi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lcdemnxd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uurgxwkd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2frqvroip.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fdffolxz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2obmjafzy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ijakeckw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjqyipyw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hehvlwrd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fcqkrxbi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nzgbddqe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ohehxenn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ddsviazm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zcsiquqp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zwnxfvvs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gyakxbbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulonthtb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2buejbbee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dllptsrh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rccvmmiv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vomtxpkg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kupudyba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2matafjrx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yuruakfd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qgbmdowp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jipztpqq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xccdsqcf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jyifsaqr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfcqhjkd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2sqrcidii.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfkydfw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eqvqhiid.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jwltrmyf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2chxcuhna.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2famyffhy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrqzedn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecdsmakm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qvrtmfkt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hpquubak.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ttcirwxd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kqcgetyt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2woeqdsmz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oamfkude.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ivjvolap.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ivqikdlm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2skucovue.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2thvpymmm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2znasnwai.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ovookapw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kffxndxw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gzcsmwyb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mtuxbxcx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ottroyqj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbxzcfg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2addemgkh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ammzlbxv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cftvwlid.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fhdscqba.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enevyihn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mniqjbff.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gbxqomxs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jwfybwcn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcczvxuv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbyssjqs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pwzlohxp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uvsinsgu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oujsxyid.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlaainuo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlajfsez.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wcjckvsa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwmosyof.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpksiwcg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kuigbrus.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2exbpgorq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ayiujhxa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2eqehhbsv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yjxmswzk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zzhnfefl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hwmdflna.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lwpwgoqk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tqfcksvl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zyasawav.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cymiqqan.html


<!-- 参考信息 -->