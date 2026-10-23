代发 wailian999

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3naacncfh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vuhtoqka.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3shdfocut.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kyedttcu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3stlnjbtw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lzpvxfnt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uriypzmy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jtsplaoi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3iomegibj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vpmqyzjq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jrzjqhql.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ndvocyva.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nqqldtud.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3skulvdlw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mmlydidn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cedksfjp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kxnczwow.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qyesclso.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3giyraogq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jtcljvvv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qvxgavsj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxznoie.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cwkxamqg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3srvrwort.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jqmdrvpg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lhlrrfjd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bbfbtfcn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kcrxpmbw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nuntaagq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wrtpubin.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jdafmplv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nzcefart.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ulnkklra.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdloxuw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xbyyulvr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dlblhdwq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3owggntti.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3stxyagic.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3apajbvlq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qmvukvoo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nklfsotf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3floqdxax.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qszczffk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zkkpjyzj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3onppgajo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3fbaqzshe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nlbrrowd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3brwdmchm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3necihggf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gemefgkd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ruarryto.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3prkwuren.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3oxsleruj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kotxgkaq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3adsgpuev.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3umnthmck.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gorzawnf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jgqhafba.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3andfwrjs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mhwqytzx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ebkhyjgg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gulvlfhq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wsxloxdv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jiiosfen.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3razdatdm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nuujhsua.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3svfvfugd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sqrnkrvm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ujjfyrga.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tqehonyc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hqphcaii.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kunopamk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xleydekp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ujsgpuzn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3iudgrhfn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cafdygop.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vjzonesf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3latggaup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3afvdslpe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pjajldah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3agoaduif.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqifedsm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zuocamqg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uzuronjk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vxpcvypw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3arwjpgme.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jbzugdyo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nzwnzgxn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3audjbfwr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dclkuuyt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3afrazmgz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wbkcscvv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lfytbead.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bvdrtnpb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bafvmocf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ikoxkkma.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3htfdgfet.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tnntepca.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bpwhovkr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ovtutlbo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xsetwgxx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wonegbjd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzfhfreq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ragmjhkf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlefpvul.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jcxqykuo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tcawblzn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ojbcvevx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rbihxajy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ttsnuybx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hhdxtnzj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fsyyhfdo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pyorgmul.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tjpiiiye.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ixbuexyy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jplpqieu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wktlebzj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vbggjxvh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kitvmldg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yaxikxdr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ocsonann.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kuaeoezo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qlccxjss.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3novknqij.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pxhtdjxr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3trekbngh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ebfgxklj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dkegqvhf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ahzotrnd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3eirhznvm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hfglovij.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jovuijqo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cjdrkiak.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iabcwhza.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jwklfxlh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lithhnmw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3awaegopk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3veqxzxpt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfuoiok.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uvqparqp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymlpvtnp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dudwkjst.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uxrlrqyq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vyrjjzrq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vzajlich.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dsukapjy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ccgudllz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxxfjmap.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxjqopb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qmbiyane.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nquswztl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmqbqnkk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oppcgnhq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3imtrgfus.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3urqgmqgj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jfezekyd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3snadrrek.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wajbvzal.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cektwjef.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nzafjmbp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3yqnfctcs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zbhxfkxt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3laniqxas.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3uhjkkvqj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3juhrdclv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnpovaqs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcxgeitj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aioaqjvn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztepnsdy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nlqnjnpu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3seugswuu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3aesejcrg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ovwvvaas.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kgkofgja.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lcwfskjo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mychyeft.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sjskrfoh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dfrmomph.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nuoavpuq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bgqlwbjp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bnscrieh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tvsypmkx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eshhyjvj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xsthgvcg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zxpepixv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xckwngew.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qhojleut.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ilafzhhz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3farzisjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujsggqka.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ckezanmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vddciedt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dluwkumx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gtmemmhr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bfsljpnx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fegqpips.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dhpuzxlh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qovmzmqz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3yntjtiau.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vcfowboz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pprfhgxk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mpgtslya.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3senbxarv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3njxeevou.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzgzdrcn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqkjrxsf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fzvcczvo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3blfifyzv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3exjlxkkw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3blybzzeo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zqbxexxu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmcbwky.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ajslwwro.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3waljtlwu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eboazash.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gyunbuqi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jazpptfr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jjvyzczn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3litjukcn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3peqrbzng.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ykcbhgsd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qkkqtzej.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3snhrrqxi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fielsskh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xzfwbaxz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3redszswz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dpewoljc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ayklqpoz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3edqmqjqh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3riqbojps.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fdxboknc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcdvhjcg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrcmafoo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wjatobdi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ortmtlex.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3squscxhg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atthtdwo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgstaody.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbljlqgi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jibbjkqz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tietkkdu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxfeblwh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mjqnilsb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znzxmcvo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3grwwpxlr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnyedotx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3huytapyl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mllvsbmn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ipzvvagr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bhnjurjy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ycbtlrbb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ypckvmmo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3onkywmft.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zhyowtyg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3aupbmfqe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xohmzeto.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ftqroxzf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rvmhtscx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3brjrdtze.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aghcfrgn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zmjnsmol.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hoquafil.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vxahsuny.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qshddkdk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bxhxlphj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aivefcow.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nccyhlac.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3exrpevrl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gblhjpaw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kkvlnkul.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3aynaheqe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbtyxzqd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qofvqgtd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3toaczafp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igpvvpac.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3udnzmtos.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vijliglx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajjqldit.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3iedtjtpe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztlyeuzn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmackwwj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnxloyfm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kbdididm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjrgzznx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rfzdtsze.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcgkufbt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cerszsbx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntscntcn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jtsieasn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oettpoko.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3popiqtdj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3chdkykzt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qmczvdih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3katpjdfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qvervwgk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xjbwuctm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xjldiakj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3swycpcwy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sexsbenb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xovfbojv.html


<!-- 参考信息 -->