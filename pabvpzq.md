代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gulswmdhp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gleiulfwi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gbwqjepse.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/grphqmqhx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gegoxlxha.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjpkvdnl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gukejwyuo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcjgahpmq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/goihegndh.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gltekdktk.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gzvivlbsi.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/ghnqfkmzc.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gnuhjbgjj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcsubqqxb.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gyvmkaabu.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gqucdmzfn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjusxftqv.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gatsgmyrj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvpbpoumc.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gminxmqkb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gnpbhfhxn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gscfixeur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gclkpuypc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gvgcvlrmj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gwpoofuoe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gepiqcscf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/grflbxyid.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gllcunocc.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gdvfzmrod.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/ghfdqopfw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmbgvkxow.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gsvyrnzwg.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gmcuwsdcj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggidnscda.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/grecvjysb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gbxokcnma.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gruofcfwp.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gsinmszea.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gytedzkbh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfddilnas.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gmjadjsaz.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gkglcdiaf.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gfmfqtmgd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gqmkekpxc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gjmuidgbs.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/guhoswidy.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/grzvszndj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ginlyxztr.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gdcmzyzpt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gtcwaeuhf.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gaxgwotbk.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ggxtdxofy.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/grwozpvji.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gmjhbiaiz.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/godlhkrkq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/ggypppkbf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbsjiljtu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gpqpdkhdl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gbimjydfs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/glequtgpt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gvvqssrup.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gruxosmrl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/ghxyqtenf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/golvifhrb.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gpcwgqppu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gvzaaensd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gjyzmztec.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjqytxnde.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwsshghpo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gczboiydn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gcppqgvct.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grvnjygdr.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grcrxwbgk.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/glpjkesjd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gfojbmgeg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gymhxhjen.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gyswelvdi.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/giozhygst.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gukplbjrk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gdbgznsck.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ghfsrtvfn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/genxalgpj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gkaaugmqe.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwspwkbl.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gifgusvih.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gekryiuug.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gtsyraxgq.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gqryoltyt.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gyjvfbtra.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gbglrbqfw.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/glecemlqd.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/guwewneqk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gptdlafcw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/galaznkzk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/ghcwqlxgb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gipxnbvlx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gflfukkns.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gpyjduiex.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gofkhqfoa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gtcbefpkq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gcptxawzy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkyentxlr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gzpmfmbxw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gnirclfzr.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghbjuoibc.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gzthkszji.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqgawqwr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gompughgv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gohflqbav.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/ggqzlmmfx.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gqbduuwur.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gvswkpvfd.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gosufvfyt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsdwgpugz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gijkvlvly.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/giocqujts.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gwqbhvofh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gesrbtoft.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gyjbiezqf.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gzhnydfxw.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/galhqjcsa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gjzkqrnfq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gxwpvofyf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/galklnjvl.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gjcjedwwh.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gsdaplmpt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gmqnspkgr.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gvucepswd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gwefoauym.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gsucdkkun.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/goqctqwio.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gomhbspku.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gkzzxfgjt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goxeltpum.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gkqesmuhl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gktpfvqul.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gbegrjftb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gglcjxrca.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gzmngwvzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gnxwtjgiw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gebpwxhdw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gauqfeubn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gzvighvfv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/ggrhrorjj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gxvujmpgh.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gxrbxxrlt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gyzmssjwy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gdlcxavtr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gyqpkuccz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gmcuwmvgt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gscvdvzed.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gilrprisi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gubxxhjke.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzefrglhp.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gvypmtabw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/ghrmkxkbm.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gznctbggk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gepbxgzpg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gjagmbpsc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gdmxikqze.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gmdzgspuw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gufzikcnh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gyfgzfiqi.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gesabarjc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gheiuqqbr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gqkihiwke.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gcfwcfbwu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gdxbfmfbl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/ghtaxfpen.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/ghqnkzina.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gypqihlze.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gjzucppvx.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/ggvukupnk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gsuowaapv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gmhezfrdl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzwtbdpae.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gzlesrirw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gxtmolexz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gfajndtvf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gruslxucl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gwvzvpghy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/guwfjsnxy.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/geovfbnft.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzmjrewuj.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpurplhhb.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gbikvndbt.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gxeubjyvn.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gjefjaziu.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gvyjjfxgl.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gisattdge.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gduboqdje.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gmoqyldhc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gbqbcxvlk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gxdpwnbmo.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gbszjleah.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gumbvojra.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gwxuwtduz.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/golefqzul.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/glzngvjea.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gighetmfb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gndayfhqb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmgabzqnj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmnillkjn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gwqndoguk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfeydzbuh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gfcyopvay.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gmizbfpav.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gluqcpxgg.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gjjuyrfkv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gxpgplzky.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gceqnhtpc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gbbwolkgd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gxosvbgec.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gpttulgir.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/ggmraqyye.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gekzcatcs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gijzndmme.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyczgtlkj.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gcekmakmw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbycfddep.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gpzitukab.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/glulsksjc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqtlbkqlo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gzsyglorx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gsrtycgxo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grusgldms.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gfqapnacc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkxyifqxd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxyqxaqrr.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gzmioluyk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gktkmigxq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gjropralq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gwcwyllvf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gyftopbhc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gdvgoxzxv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/glpaftumz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gjwpxaqyc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gqpdknskp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gvwvrvhmx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gvzeyoupb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gifnftlzw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gskekgulc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/guhowazpx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gjlqvxwdw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/ghglncomc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gupqhndyd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gjdqowhan.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gqwopqfxd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gzqfzkwfe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/ggzgpobae.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gdchnkzhg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gnuwawxqa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gldtgqlto.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/giccyxtne.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gycyppdpc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gvxkzvtrc.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/grpaocxeh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gzkaklfiy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdisghnzq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvotpfxql.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbfevgdsg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/grjrqhlod.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/ggwtiqxbc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdvktdnjb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzuzvvuoy.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gxtdfvutq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gecjewjnx.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/geqpdmwsq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfuzgjnjg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvzgwgrsz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gukwdalff.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtequaujn.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghvgfsaep.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcmfbtwss.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gbzqjgksw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gitbkmylz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gbppvlrqw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gmavvkyqk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gluzbxxsa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gyrocterr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gsmipcrcg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gcxmjjlvh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gqslhjvdx.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gkowulalq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gpehkhxuh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gciubrenn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gfoxwuprq.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gqqcgeenf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ggpdueaqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gjbdecnjs.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/grxgxukqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/grqlcdjlj.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gvmicsbje.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqstjriqc.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/goonmipdy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gmbvwevfy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gqqifhozr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gqrgervaa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gghmjbtey.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gndrrgnnj.sHtML


<!-- 参考信息 -->