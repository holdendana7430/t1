代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ksxmsifb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2witeppfd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bqlewvkz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qqbvmfwb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2urxyldbi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iechtsuz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rdjtjkhv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jesvmtym.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2byvrlrxq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ulckizxw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cemuhdtm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lgrbezkr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uvywrbbq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ednvembd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rifcnllj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2erxtaonx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tvzjwcjw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkagkxvx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzklfkzl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lyjrhmei.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rregcsjs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pcxzgnji.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2enrmvieo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fvriudxg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qwxbkisx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ibaqmxxz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uzvwfiuh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ucmpfonu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyscdypm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bukqrtfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgjysknl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbdrvuik.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2amuwasmk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2txeqoulm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ftsuqmtm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iiqdapdf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2kjfhjfos.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nxmmqwku.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rchoaits.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dcpyiink.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gjwlzaaj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hzkcqryn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wdnbvmmu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bkovjbdf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qjekvdqa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdujprre.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cqpwtyhd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wbmrrycz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2upjyytzf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jltwvbkh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2azhrmlsg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sehzzxca.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kebjwtxo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yfzdzbew.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qfotpwsn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cimmiydi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jdkevorh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mfzpnbdz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qarcphiv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2oqphrvth.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2trhorvcl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sdiixytz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2esjstbyt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2isdfnwfl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ajxqybwt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mkfjkytc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hdtayvwg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rnxkkngh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jvmaxnet.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gcsykfif.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ngpqrtwb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2edoophag.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2goduwmwx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yakuscqk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mhwyuccl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2schjonzy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zoiqmbbd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qctvbecu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lbiocckr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ryobjyua.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cfzmtasg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2crltngax.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vttvpchj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2odumanaj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nhfkudwb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lmgmdmow.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xhshfjwc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jsixhkra.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmnkkcp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wvztzwyk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bbvuukfz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2uxlbvdds.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vdxwtgof.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lzpbrynn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2iwkwrkpy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jvdmrssa.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2itesaefv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2epqyerel.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mqxraawg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hjfjazof.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nztbxvpk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ragvrbjj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2afykmoym.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vaketdba.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yhcnnbkf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qvoghzar.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hebfcqjw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2evnhvgpo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xmgvrnhy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pssszoxn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2omkkncky.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sqpibalx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2oocbkbfe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hwzozcne.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2peoieefu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2htejukui.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2quffefbt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xkepxiqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zjbmojmv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jgwosfbe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wvkrkabl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vxsugitr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qqrvihav.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yngkvamw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwicndd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ppcoksls.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lrdyzbvy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ycpvbomb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fumhkxdi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lskvzorm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ehamkgkn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ktqbeslx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2swenwkgu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jyxzuvno.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fotmrete.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pmmmsttt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qffswioa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xgprtimf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cufeihyf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wwwmvktx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qbjzzufy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2djqlaozz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tzeoccfk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rcqngllw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pwvzcwdf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2csaorzic.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2shacncfs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2utncorxa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2andlehgu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pzgbsvbs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2frdxqudy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lfhemwfx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kveisqqi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ayadhvfp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vzansilf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sknessox.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hgirkrtu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2udllmqdc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiyqqal.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ejbfarzi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bcklheqt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xahdfcxr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2acwnthzs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pdlfpbuk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qtvjfsqm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2duczzmkj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ypjzwjmq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2epbkvihy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2unblohic.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2teueivic.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rrdaqujp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ioeccmrw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hopvuxoj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jyknbbmd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sljyjeqx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yfcjlrlp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rihseevk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahsmaiwy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjwhwzc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ljvnnrqt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oihvylgb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2oriwlgkj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hztjjsun.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yhejzogw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wsqqssqb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lzkctout.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ksahaflp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qigaeltx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fwtetoto.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bulqangd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2btkitaxh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vwmdnwfx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlmugnyl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ofvoilvz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ohfipvvv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2earkpzss.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jbdloxqn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eenipbhy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2borzvfmp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bghvdoax.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dqybrszq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wkxsfiof.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tozwfvzc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gsmsmjcs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2yhcwwsak.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axvljjyj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjktgsit.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rydekkhl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbdrbpeo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2hikvtnuj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqiuwdcc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gzjyujae.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2pedahsse.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mmgrehaj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wgvqnbki.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vydxfgjr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wzahybmm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2sqdhukrw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rwdnypzc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bousailt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2pftvyamh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnkgzda.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pnagujew.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eomoexgo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nxrmutmr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tdpavmdu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hbkcdixp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xnluxgkq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2blpdgpfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xudrjfga.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qpdoxxxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjchbbrq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cigblhhh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lwsbkefs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imeiygbo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2brytyxhb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mxwloeon.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nbbdgbxi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2iygymxmu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgzrajcs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ebsayddy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fcxdqmks.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2akpleteo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2nkddrdpz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iujpkgsu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzjtylxy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtnkcju.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2poxntppa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nycxlznv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iktnsjpe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zkaghlax.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wmtoakfr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jadyjuow.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kmagwzfl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ivtryutj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uordvpoj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kkruwjpy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kxjzyvui.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oexbeyvz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ssdvrpqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qzldacuu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2blwuncmc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qfkcjfly.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hsfzdxnn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2szytgcdo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cangwybh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xhbchhxk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qxnzexdj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2pqyodewi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kmqklhbe.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxjlmrsl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxdvaifl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvchwwtv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhbkinpx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qwhkireh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flyokong.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbjebgdw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjdpnebw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cabofgpa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rdmlmrnw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wirqlzvq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcbextxu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qqtetjic.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qybaonbv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgurivii.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gwrisxmk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cqeyfwtj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iwjrbjkj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2grcakxxg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kugotrek.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ogrezlxy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nacnlbzv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2doudjcbl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2shoxhgxr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2djfngsia.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2yiforqcv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sstrbwom.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rklmoxzg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tdjjtbgq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sklcxwno.html


<!-- 参考信息 -->