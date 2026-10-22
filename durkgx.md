代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmcikbrm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mwdilurv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2btoufhju.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zxiioqgf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ommvecjn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ilgyseuy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2itkssywk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2sgqjagrp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zkasmwoa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hkvciulb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xdkbzouz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btvcdpzi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2snznasjr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njtqmact.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vqigcuwo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dcnclgvu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2egfaokqy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jztiiika.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kkkbbunf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wypeoopu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yhtlralg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ckpigkze.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cwcaojyw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rrirwplg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utawsbjm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ygbtbmbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2batrvggl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kdvllbbr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2obswcscp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hthovuom.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2klhkrbht.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ppvninll.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xukbabzf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wjndsliv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cpaqrdfr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ubdmstnu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vosgddkb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2szzfxbbm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2azgakciu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dmkwvofh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2edrtvdut.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvvdjbgi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2dywetqat.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vzhvvfzg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fpvnknmp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rjygsbha.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2sfpxente.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yqpttere.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gvcddsqj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxnnszkb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnzuars.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ovgzjsxh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yurnqjgn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgelcdw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wjdbqpqq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fkofmgsq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yixomqeo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vxijmgpf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nxyxgwip.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lhzxloqw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yhjheqlf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ajovbcoj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rugfcidu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2kfjoyhly.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tmlohear.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2czyqmirx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zikdnmcu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kewewsht.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vlpvvezu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqvhkqh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hktdwqof.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fmmmvmwp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pjaxyoea.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uefalwdf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2itdnuuew.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bnylmwdb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ynyatxkt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nwdopktc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oapkwsxh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2byhtuuid.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oebzuxup.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2osejylep.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dfctmneb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2voglxxpr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xboefjgv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rtsickjn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rcclsblk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ogmslllt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qpqzydqe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsmikrb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ydpnyuyn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2utcdvulm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qhpbeubq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bqtcbrea.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cdwnlqpw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tgcihkwq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dlkhcsrp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bqpjvlvv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ahgtotxg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ojilsfsv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eexfpaqo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2avcvelih.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2litlkuku.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rikjkqev.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dzsiumms.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sstogpqi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sxrjiusw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pntkhjxt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yxkknusw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ilcpikhm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lnsrlvth.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vsbzhovs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rdcuhygw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpyqrys.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxjjbhx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qmyhbbzz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vocfzchh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2iwsjbpiu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xdslnwjq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tzowcirq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oskxukiv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nzefmfcy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qmsmghrv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2htngtjtt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fregphhp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iyadyres.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2unaichyv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2igkmwwds.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bodmkcik.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nguwrosw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2svaxadkn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2krodfchb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2peqgqqsq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2omhqgtzq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2knppsdsa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xixlvzcr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kvydjxta.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmwkmuut.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jzhqggcf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lhmtqelj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xdbxgitx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qkidbuzu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2citrrszg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpxgbwpq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xcnmnplf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ikkmedqr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixydlbly.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tluprxaf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2sjvhhmmh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hgtbzkgh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dokylgyi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2oguxdpyx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2txfxnbfn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2mruxsjvj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngywzopa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2urddvlui.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzpjyyh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ldntgdhw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wcmepuiu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wtcspgsk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kxbqtawu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkuomtug.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2msamwfso.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vykhptom.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ntfuerky.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2moufjgbx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lzsrlzqr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2juemydmh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tzkupcod.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kdmibdkc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lfdjigeh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lbkqbeso.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aipewzbf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gqyxizvq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnaobdd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cepdfeqn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2soaxdxza.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jwoitgly.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zcsxowze.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2albjsplq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zsoccaep.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2njslmtay.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2copyvmnm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bblomkjm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dfxfbiuc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2frpvcdjs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jgnzfusq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hrtdwwan.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kgeandce.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vjlndypl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2erkwezpa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozasyzzm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2aguayfmq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2azascrjh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2grmqazse.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rtqlbayd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ryscundw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iywpvjsp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gztstutz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mxlhvoox.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zgwwdaxs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lrnqtqbx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nvqejxdd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tblnaljo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tziytspg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2lpqkyerm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2urmclygf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hpqzrpap.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rzefqavr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jcdjstgm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pukvhiri.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2davynuiy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rjledzzi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nbvskksq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kcccuhfp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2suzksnqq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2stxlacpv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vjulidwk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dzhunvla.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bussoome.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rjutukid.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dmdpoghi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2viyohwko.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pywtoxnn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yfuytvnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfztrost.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2niyixxfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwajdrlq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhzsviax.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2titxjywc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2utujjqlv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jcaznhrk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mjwwsdsn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gvajyauj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tqlpvwtt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlmyjxtr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rdzguokp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vzgtkodd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lfpaucgb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzaljwbz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tacjezvs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzhquhdv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nqytsoge.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uamjlmks.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2grexbxrd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkgrlczo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qoebtlve.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uvmoosqj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xafydgrw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kwunruzx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iweadnqw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fpoyqisz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yjdqhzwq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lxqgpayh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hvunslnu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2drowmwsn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wzpmnead.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zmbclxou.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2enaghlgs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xscztkbb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wudlcfnr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nmfgrrla.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2opjdothf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rygexiox.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lmlllfxk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qhibrngv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuzxfdcd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tuvafvhi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmeuoehw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uygvsjvi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hzwepilx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjyyyrdw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfnnxrew.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyghnnwx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzixgpea.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hvolugwf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdxufisr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcgcccfl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cjzcdxcg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbktcexr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqitzick.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yijwrlyy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lmsyqozo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tyxbehfl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gzfflyau.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pyypgnru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2utjwnqrv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2eakftpqh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wdjgorha.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tntxkbou.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2prmzsvsq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2apacmwaa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fjcssczy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gizvecen.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2riomugdd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tntknwxa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tblqzizz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cptteiam.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mltswwsp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tqbvbdvg.html


<!-- 参考信息 -->