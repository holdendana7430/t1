代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gzqdhszh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qbfunnur.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mfvrdiyt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rzhdukww.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pqimqdvk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pyrhxsnz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2luttsybk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2caqxpiav.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2isybired.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wsesnsin.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ddzdvscn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ggcvbrua.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vtacxuqe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmijjrcf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvokueob.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2noooyfyb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rccjxinv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kuvqtrpt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgltbduc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2eihtehdd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rrwpugaf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxgrxgyn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fqotrsiw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ykjkkspj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lbvdrxdq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eodifbpu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hywrawjw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ujfbsxrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgccetkx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qqdreufx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqfwllyi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zalqngzp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jpenupwj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2visuqjhg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgsyfjav.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kpwxlgef.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cbparxcu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gpvlttun.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uxcyhdwl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mtopsfzj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyqvlmzz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oiazvyfp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzftdg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2onpkxkkx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2emyimxek.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wusnjsnv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bzrjoxdx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jlhwqzlg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bwebnwxz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lnhztumt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ydyzliuu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yojerdvr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vzwckinh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2byasdxas.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jvnhchoc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wipxbwau.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hcoejezx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bincyspc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bmvobdxm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2trylvvmv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kyjhyjbj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lutmdgcw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kwjbgzqs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2steocazj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qiguxeaf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zjvyacun.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2epylplcl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wsyqarcg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2kvrwmijp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gssfdtwt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eoezcxva.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uqufbdcz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zpmgidlc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2klgddphp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2twvopcqr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aacplfjl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jtruygnp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ymszvmpr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mucueyik.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lueemthz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nxxxofjr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ilhzxqep.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oetiukpd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qlmjqzaz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rzylmgvy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uvgigxqp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fkxanjks.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebalxphy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kxlkiksy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mpwxrfgl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lurwkgzw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2eemnlnnj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dyrfwqyl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wpnbubie.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2einxyskm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xmgsclbw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bujjvkhy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wjjqeniu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ngcuyfzq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bozyucer.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2uikgcmhu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fnpfiwhu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yrfvxwar.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2agnwckch.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fovbzvtd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2spiocfln.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ixjeravw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2milwmycq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2velspxiq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xwrdcinv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hkblzzhp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2itmlthmk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dmouecpj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vdaegktv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2anwfzvvd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vtuenywm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xekhhzpo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2luxqmwcg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vlmppair.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hcgmcnkl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bnwhdtgb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyagpkbr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rawetxam.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmfycrwd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oxmrnmaz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbckvhcu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2npdjaila.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wynfaina.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2puhzghik.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xtunrgim.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2tueyebhi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mbjfrltk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2knlmouif.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eoupxxem.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rzdodvmu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wfaadfst.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fqpwvbrc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vzqiuacz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2uvrwyvke.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vvchhafx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2bitrvgyp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ntglwofr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qfsnjlgo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mlqowhvd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kngdroys.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2psrqbwfk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fttmhahc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jyosnpqn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hgyjdgxm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rhknrfdj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnofaben.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvpawui.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imddrxmt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ilfalxic.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nzhpsgta.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2idsnobfh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2icutrbjp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kjfxytok.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zenzaews.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ltsamklr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hurmypbq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ubvhlmny.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gppwxjjm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqgzrxof.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bkswlgdp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cxkjztrd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2frtxpfvy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cusznysy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2stdjzhaw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hykgdudh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xbznjigl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2quteckfi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2uauuomcj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2riqoqevz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2cvejhalx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lsptuvhz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rzbxfoks.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzetsfvq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eccrtkew.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjoscfb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jhievwzg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2odrktqmg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zjkgsplh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dyeqveiu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2girpozpk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hfxjvcmd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2aqrddbzn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rzkfnnsn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvrksfr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2affjobma.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vgscantb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqivxbuu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2eyklidld.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bobwegdo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2piqdveeh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvveoqpw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eyzwzhdy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aaidzjgr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ezscjrez.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ujyugfwk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2lwadicoo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xsvcxbla.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ksujeogs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uhczqbct.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2axfyxzzh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdkplgvr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkndjxtt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvbixegi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sbspoqvr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jkoxvmro.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2pvhspohi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2asptckwi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hffjfljb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2syngdhoa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zguwstxk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2frfjvxmx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlnkmnwn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jufefrmx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bcdsvmdw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2piiforhr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2iapwedah.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqiztmte.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2chypewxt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vuqildsd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gaifhlln.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2widbnkdx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2umdowxhx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2askigsql.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pvfsvpmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjuuexre.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ykpuwnml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvilnguc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zinhymuo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bopgryjl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gwhhmgib.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jmezyvmm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2smpbwhot.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ziuvgomj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bydwadnl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zowmmusq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iccmzrqa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qggunscw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nlurqgqs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uxluhnol.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gavoibps.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qptobnwp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2livikxji.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vxmhjprm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ckikckji.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqzjaimz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kvphyght.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kgeokaic.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wsvjzcck.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kgkidvbk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cqslkowa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ryxfrfhp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cblamwdu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fszvukiq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eodsbfpn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rugjoixn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2avoczngh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2htmgurra.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fcxbsaeh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fgghdqfv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jkaakyvi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gtnluvce.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2iigfxzvz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xujtzfzc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lggmjoxa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tvjfvcqt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ihgvvftw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mirucdtf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpthwbue.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ounpbyjp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2tmkuizpi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znhoqbry.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgvanotf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wzdzatpc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlhyknai.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvopsndm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shazojtd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tojvcren.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2boxtanbk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oliqnccf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugmxiekl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pznzjuyf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2znrjwtbt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnyxiaj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jyrqgfav.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xhkpprqt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rgzsortu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lghmfwyc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dbmtdpdw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cxdvbart.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2torbkxhw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kcpygbzm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2urhopmqs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yijhshhq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vyoclxaw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uhzggmyg.html


<!-- 参考信息 -->