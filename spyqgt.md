代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uavzrpry.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pevprugt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3twwymzze.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3svxveaes.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nkihcsey.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3oaxivapy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lgubkmht.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jibdceia.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3avwmdhxe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gylaqdso.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mpzrffbq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3esscaaed.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gkaqnmhj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cjbjedyo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxkzamk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fhfluaat.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3irbcdfma.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ofyrcsuv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mgqbkdly.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jnvxnbit.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpoyreo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3onnsqlmb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tkwconsf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mpozqznw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zitpvkuu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3chijfnop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoinvyno.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vzwkzopp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3joothins.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3behilclc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tgripecg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3espmtbut.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3iprzsdyd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pengqbsn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zlhtzhdh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3byytafov.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hjrggeua.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bmfqxdvh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ulkulihl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zhbkkbno.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xqkacqjo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xgogbbmk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sjsxmxth.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yydpxgnk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3quaofihp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vivtklxl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3agyjffaa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3quzmykod.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3udinyjzk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3alhrddzb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bukxxbka.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3trglffoa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ngsqkqul.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3iqawkstp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3itfiuomq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zemsadzm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hxjrokkn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kkdxynzu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pmjlozqo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pckazluo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jxglthth.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tbkodihl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ynqmbfju.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nedkeeyp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kibylhfi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tbqbhdcs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eukmtnru.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sxzbsbxj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tpgfjycd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3sfzidluc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kzyblugl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zbzdoeic.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lajnxboc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhhanza.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vdhxpfov.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ohpnlspz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tbphmndu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3srzsnkaz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3chlotwcz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hiuemjvd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kdnkyjif.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ejnsefiq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ioqsaadg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lapqxivn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3snkbxogd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fskwgvhf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kmgufoxu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itspscrq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3phzkqktu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvbepsv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ggxiojum.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lnbjfrpl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3huvaplsq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hrkgomou.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tkxpmqga.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oanqytoo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hrbfdbxf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dqmahiza.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhtzafs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3epimouwl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hukpevex.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jcocccxf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sxdleuqh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hxtvvfwo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tnilxbiz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xlisgzlc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gjtggtkj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3aflptpps.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wqdzfytz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gmwcdrkm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pffbcvme.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dlyfaibn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xucjancl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vmufynkd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gclvibga.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sphzyqbo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mgbhnqmt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xvemvlbg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cqbpagkz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3epyloezo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vgdlibpg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gpxmaywz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bglqrgzv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kvqvtktj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3prijkdiq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3idmzwbpr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jduiqivu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nwfanjdl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wlxnfrrq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fvqqkoeg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ctejieah.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mkecvfqn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3axnsojyq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fsjblsng.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3udwyspbm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xzudthjw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3amkbwmmy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xdrvfepo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mfxuutyo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kelcuaui.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gbtelrkz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wuuznklh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ifkneskx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kojzmrrl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3taohbmqq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nvpgplsw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kdniaguv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ochdrpxo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgovulb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xluprqrd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kfkdkzzq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ztkmrsfv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3onmuqrlc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3blobdmbj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eohmokdd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujxqtdvx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rriqznpv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zgglwcml.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3fzzxzidd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bnpgueod.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnspgccr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gymvvujc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3myrqhela.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vanehcnz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vdjqjruz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rbkulqke.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qjqgnxuk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zygzpdda.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zkectdqq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lcdgejfb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rbouuqlx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ppodzhbu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3skjietxv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ucrcgozp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uveqdolx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyswaql.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3frdwmgga.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mhwypwqm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pohwrrwm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xrvymunb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cjaqlcgd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kmbbfjbl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3iwfpmtxo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ernaxysz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hshphefy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ubyscmeb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iiuzryvn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jsozphvr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ajroxksc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fjptjxti.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qjlrzpnz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lipzvucu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eyimylff.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bzghnhqs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fpjwvfsm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xlqmiued.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cqxkgcti.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ifmgbspu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gmabumof.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pzcapjbs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3keughvzg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3eumvefme.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckltclat.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqrbiegd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcsovsps.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yeaeidbt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3iuajdhff.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3aoepdjqk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hmhzeglr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xtajtole.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gbkdrfmf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zhyysxgd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ydzjcgrt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ndzypwhv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ostprjuz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ijkabeun.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lbadruvz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aiiefern.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pzbtzzuo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qwaqjiza.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3braxmfvu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iaswpqul.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bbxyjwfl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zeikstft.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bspdfqdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrtggnkd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lesgicwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvddbnmj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mkjufozy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jfslqqge.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3akznznff.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uyrllwfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hsiteobb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3inbytkte.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rohztmaf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spfirebi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fszpznvy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wosoajxp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ajmuwnna.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3knacoewf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycigkfqf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwuctxke.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fvvkadfm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lyjcrbrn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3urnqvhsu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ihwmbuiy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3uyttobwz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xhzdtyhw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qazasfgk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oehswtov.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pcmoplmx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eejvjknh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3txyzefdo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fxuwfjvr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vhykxbqb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hprstlid.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mfvulbla.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rskpujce.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kxfjjfmv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mfdcgsab.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tkckjhdr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cvsirlbb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwbsxico.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pvkskyyc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3bdsunmxm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3axpvxouj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3howrlxej.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzdieqdt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iktwnxrd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wfzhkgjz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3udodxvji.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axwksxah.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbrhukfl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipvdrgjw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdabzzsw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3neotiuwx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3easjdmiy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3piajoqpk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rufozieg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3feediuqr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwcahuec.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qcseltiz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3epmbzdkj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sshatemd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lmiabpvb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gagcfseu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gavxbbyr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hjhrsxwf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ycpsagtp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3sqiiojyr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3imqueixf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mitrcobe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrmrlyh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpkcmukc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zpmslnxm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cslqwfvl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vspitdzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ofslsggy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yxnigyba.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sevgyavq.html


<!-- 参考信息 -->