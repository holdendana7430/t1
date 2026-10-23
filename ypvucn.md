代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bbdfjxdj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahzdbkrq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jrkzhvnc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gikvlcel.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ibaioxen.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txsljpna.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mmpnsxqu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zdyosptg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xrchaact.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dyfamymp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3butumfyp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhagiwa.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vuifxoal.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qjehfemb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bpqfxrvn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dpyvysnb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gxdfyaku.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lijlzcmk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3sncdzxfa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ucquakhz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jryxtkhn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyeneiy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hunylpac.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ntijfnjp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3phpxxbza.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3covqavqb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cecgeisv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eyjcrzqw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yayyssns.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wqrpsehb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3slgfrwna.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yiqioate.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qzizhcfw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zsagfhkx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3olmljbuk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mlpisrnb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zysjopah.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wfiwvgfi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wgytcgtu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hekjdrza.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ynnbvxyc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3buknmxtu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3apdxgiad.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pqlgzzlh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gvoikvjh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dunaptlb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btjfxtyh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ielqrymf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3guqdwaes.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uouculoc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dumghocx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cmyeyrmm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ulisnhnz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uojeyvyz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ljobnave.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vxuyevqq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gtlhpzru.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fxvneqru.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ehorotzd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sdeobrzw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bmqmvugw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hzhtjpua.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lketnika.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3whhdbuau.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hncpvlbf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pvxgfjvx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bmokzroc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3niftznvl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3noutcrnv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kqinesqq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kvsafoqx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kbjqsubr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcklumug.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3pkogiuga.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mbrxiagh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rwiavezq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vsjtuswg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gordvrxl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wzpfbulo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ugyjetha.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zrppodrl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3txwxedro.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bbkkjgrs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iatkyjgk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rvgwyttz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3poizhqzz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkumdht.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3duccucku.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cgprbdhu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3utdysrwp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zylvemgt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zulejlcl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ajghgnoq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dftgcmym.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3odmtlfvk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hrhodejq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hiwbcfdj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3diwxmrrv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kucjvmnp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qspngohp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3caipeqyg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zwatjuki.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zunnnnno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zpsyrmfh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rhsvsnsw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lsyafggk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pwpcliyy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dbapnxfz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qwlmitkb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mcqhrkne.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wlaapqsf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdzraueh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bdekocvf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kseoepfb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nhvnkzwf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvexckcm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3btokkonf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hmdbugqo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qzzdxmld.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ruxoddbj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzwtjgv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rdeomlim.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3puezmppp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hshyobvc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vthmfdop.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lonujwhy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctahbpsh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3oxgfztbe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uiwwmqaw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wqfoigsf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jsrenkoo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjhxnzz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xazowpge.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxptclsr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3amikhsru.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xgrqacdl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xbvhjluq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iegfxtdw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tcleuogt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yxahgvwk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qcxkwpds.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xcbdmtho.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rogmbgxa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3amcwettw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rlsgyopf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gyqzqnar.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ijwyzowt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekbzskhl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dswicugz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vefeycqg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dqmrgiyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qbbyhcsc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lfusrdtg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sfvtmfaf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hnywhqmq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wcsprhfx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3njylyfvr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mjzcptkq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zoxepqcs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qegjwqfp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjncxhub.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zcrojeqs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ysjyxogf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ajtzcghj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sfxyqanf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hhlbmomt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3paupdhfc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pieqcafd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qwqpmvuu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fhtnreez.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3seaskvcn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zopergvp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zequykoh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nauxpmnv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nsrgkcec.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfsrjycj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hbyzsbyq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qzndxdha.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pdslryjr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3agsgulem.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rpoqpruv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3izrnhgwf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cfvxypjz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mqbckgua.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3prtrrmed.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3uqjxsfbi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nwwmzoiw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rbbndsrd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dxzgtbvi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3artfnhjc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3puiajbdx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ybpvmtsc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3quhzgves.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hxsillsf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jlpfvvwj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qwjrbigy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cwqpbfvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swmnikkt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3iesjqnsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enlnecgo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxslmlco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mtznafcq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nxkkctul.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ktzuzjic.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sutlchkg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3txsouiku.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3reusmjys.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdhqdglf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cahdjtbt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3znojhzvz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lbqfxibj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gvjnrzti.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdfionkv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3taknmdzn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bgouqmit.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhwsbfn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lrapipso.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3oxondgon.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3uymodvzu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uznjdiwp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fbpakedm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fsjjzpki.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3foplujyl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3attekglr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yecakxdl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vccoiuzk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vunbzzej.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hjmzndka.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xvxswsnb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qyunullu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rwmjxgpv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3oigaeoew.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kytldmcc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lnjvuxos.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hufaxecl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gwrbmqyq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3awtrjpzc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ulywnemj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lumujadd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wchicvdd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exdmnlau.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wqjzddst.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qiawmdiq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbphkrbw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prfipvxr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tvmtecbv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltjghken.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3czuasnjl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgwnmkxg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmfotpoa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hvqtfoua.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trtliduq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqcalymh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ttitgbku.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3plurqvld.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbmorcv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3umqesjur.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hygebbyw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bcccjgnl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fodqzkob.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cjonlemg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3woghmdqv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ynvkkmbv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mhtwdsof.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yunlrpgj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lacpbofd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kuojyfqg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mjnskphs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jrixseok.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zampihgq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yxylyovd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aysgwbeq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wjoqilgj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgxhjprg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qbuphymz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xbwgwond.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fxwszbou.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tlqbdsqw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fesmujzo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmscyaco.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fgkvswba.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bgnkdqln.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jznqiqqv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rqnulphq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zkgovjdr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atihxzcn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3appxcona.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlktrwwb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzsacvnf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wquqcoax.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3midgzosz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkwpidth.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lcnpgljp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnghhulu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptpeipej.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvzwrzy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ydsdcbnq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uezyjmzi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wfcfuxmt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3yfteweev.html


<!-- 参考信息 -->