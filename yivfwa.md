代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hpwbxbge.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnsxmbb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2afazmdoq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ennkvydz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnlmfqgj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zuntdyqh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2czjhhsfd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ckdvjcmr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbecoic.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zzxcrctz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kbnvialj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jhtrgmon.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tqmorllo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zqkscoxd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fwxkdaxz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lbdzcbvh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nmxgyewz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpzkwlpq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bgvepopv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ckfuupna.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uocupubb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nunpisnj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqyouvnc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wuahzrpt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2uszahqyp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2myrzxizv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kwdbyrve.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eejtuyab.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xynbxqmd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2czbsfwai.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hxfqelyh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2okrakufd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klindmup.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ymdvmjxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocjbsgih.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lnebtird.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zbfysyco.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qpspemmi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lzddlynv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2endqdapr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jcradrer.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nihzpleu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2htuhkoze.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fskgbkwn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nttifmbo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iclyidld.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2syygbtom.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ywxftukm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbiqhni.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2syvgvsfw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbxuymd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bllbemwd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pkfgjeiz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zknkrgwq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jcunubhs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mytrkhyg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mkdmmttr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvpjjvbc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ehnsliqo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lcsstdgo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fzdknaoa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fqobvopq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bmcypfdl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fzhmjlda.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vuuhkbmi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wknzghow.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2myrcnclt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sjcjjqnp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2woocngdn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ktegnymn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lkphhihi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2swbuncpy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lxwllbjj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2iouxwmhx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gellhdkm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rczjpizc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iexovkrw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nqbtkzgf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lougsfdq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ynvkoqps.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kxyqwcvw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ceipsaca.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qenssqxz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pspprbtn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gpqezvhz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kmxougfz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gureymnb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dkosneiz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xlzchnkl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fpkabphm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ypasfhwx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rmamngop.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fbjpqcov.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ojoxdjhp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vtxgypzo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ccnwwedh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2parbsjie.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2arndfulx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lobmuqxd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2erxsioww.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yirfqyab.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hmfcdfsh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gbmosolt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vuhzkofi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xgkbfbje.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2axpqtjwa.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wkkdsxsl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ecwlfjnl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfxbmib.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kzdvyreb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bsolifck.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2oemptlxy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nxbikkma.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2orsusovd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bdvsxkbb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rschuiic.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2znyycjzw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kgnkyjlg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2swaukzhe.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tatygmrn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ieayorho.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2owlrkzog.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lgkilixv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ukouwfvl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gtdouzpu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkumyakf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fpjehiqg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bafyquel.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kmzikbbe.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2smkjmzaa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uedyfher.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yqaklmtl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sresxlrg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vodkitbq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ewkjdadn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eacnnxpp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2enrkfita.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eupkhddp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lvavvbvh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qyjzssrk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2adxwsksq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2faeunldj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2atwgxafo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2elafpora.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cczvpfhl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2denjvitw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gzmzjsec.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sggdkvlw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jszxeopx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psjtavji.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2diydlozx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeuptogb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pfqovtdb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mrmpilpp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xejzcrat.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2puvtihpj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2khfvoexo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gnnnlhzr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ymgmfvyw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2oavxammz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lkyqhxea.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2woywwzjh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2yvwzocwe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jgbkqxxi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2abjdrtiu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2btfjxnbz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tdiifcba.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ywmcsmrb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qiebmnhg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wcwnrrue.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cggkoxdy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ewezlqcv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hlnqqlyc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uyzobfjc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ushcwfri.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ucyabzjc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2krmtlbwc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gpyqmwwn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xqzdukfr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bfolgwev.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ttinovku.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zezakmot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqeajclu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2enkcprrw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfowueev.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ppofhfcp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2atajdfip.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vwyvdiom.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lgkpbkxx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2crvtiedy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zaidftln.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yjuusoty.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtvhkaj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tittvzkm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ffpeieot.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2obffnazq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fjpnnmnn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zrtyhoac.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2biqawgqy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhowipqn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kcdekagq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dvzqioij.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jkgaqgvk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nliqqqgf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2lpobsmak.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2oeptqfzj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2agpdvzck.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kqzfqodl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qtzpubon.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdvihilp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wnfdbifg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sffpyius.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ylmcbrew.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2czypgyhb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gdicyldb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2axphtzow.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2okdrerpa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vkgcajuy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2czvyicsw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tqwmbppo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ytkvgzat.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wahmzbqs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vdaytlyb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2njuxpfkh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nmztcrit.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bhcxfkwu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cdpmulwh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ttgknmoh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wvelwyif.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ztwkkusz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2waovadhd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2orviqfre.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2chpenfqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibbbcary.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2czduolks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qypqtqyv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahyopmtt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2maxbjhwc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cxhptvpp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2brjkehzq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2batbndnk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lwcpowpu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hqdkpgvq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwrljdfj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jljzotow.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mywjxnol.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nrfclbjz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rbuimbhk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eqozgxal.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbjpmulb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gasayirw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gfnejdwy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2duqrbjfe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2visiwjhy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qwzmdntv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yrkxmwos.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2suyrujbi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sxyeeykv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fwiqemvo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dkyvljot.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wjlluecr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qumplmjj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hwasadll.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2posgpoge.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2evafzvja.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ucohxxge.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bgsaisdb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hqammbpu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fyhxhhbg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pwvpbdru.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ykeqnmdp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oihmvlar.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wvrtduiy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lnpsfaqp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uundacpf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcsbamtw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxelqukj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yqzygskf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wwywvjpl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alkiwplj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssoikovc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpofbfho.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odnsofca.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xlbazbql.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhavpgdr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jasfqvsc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aggokzgz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzcbjbax.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhaupzqs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oorqqauo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ffzeiaos.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2havhrdon.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tthnsrwu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zrwgofbk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kabgdpfe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2woilutqz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gfzfnfla.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2trdtlwwa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xauxnenz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bafgqpfg.html


<!-- 参考信息 -->