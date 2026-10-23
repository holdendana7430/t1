代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vczfyzpn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3doltdwjl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dwxshrlz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dxtjefdd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bggxtjuo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ewzpsxts.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3abilmexf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pdzmkhkz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3sdzwadfu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdqjbxvw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lqpxnjzh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gwogdllu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xbvjjgjm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vennjacs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xnnpuqul.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oxrinhhd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3snotofva.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tfysspcz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3trrykzag.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bvhukiga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xojbcssu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zqhyelfh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3allncfaj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zxzdguxo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jpvfblmp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fmrbrcww.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3buqxlbnr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vcznlpya.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hjtclfcb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkdkpgpu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jmyrfclm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yswhjnyc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmdytgat.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uyvkoara.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxscrafr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3prqewsqr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ppoeyvwz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nkzhbikd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zebjghtb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wvocrmww.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ritspjbp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wdnvrqve.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ucfzbipv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3grucrhrz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3oxuhjsut.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jhhkkxim.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lwolsvqs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zyodwjdv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hlovbfas.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxcfdwcz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qjclreda.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dnohqoam.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zlteefmr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3agnkkglm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ypusgjjn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rturhgac.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvmxswq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ldvieldi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bjebylcr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sbnhgezv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sentlzcg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ximbilnf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hztlcvvu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tdesduwg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kfxwfyrp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tjqksguy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rojkubra.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qwvhkhqw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pqtskmjv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3juylbvlo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwlpydk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3frvprsvl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lvvwqoph.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bldznmjw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3stermssw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tygxkvdn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ofpiztrs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xiavzpig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bplbaxkk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zkhdzrxn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xraqftbu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3igxqcwqs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3igxwveks.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pwcqsaxi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pchrzblu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fnjlfhty.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3epxdoxgl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3emzxnytc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wbmjhovn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qnixltaf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3svrxsjok.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ncjhnecn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwexknu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jggcqfhl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jfvvybgc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jpmonnpb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hsdlkbyg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gvtxrfiy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rzdupkin.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ewrxqcvo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lxdlnhjx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xgkpfgaj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xnakcqhf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3makupvhq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3boinfpqx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhjxnfc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xltnzzwd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oaztqewv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cvhpsizc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ugeixubn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neogbotz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3tzgbnowr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3syriwomb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3henwwtub.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3bliewfmv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnxflbqz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhyytxg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hvdzbcsu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zrizlkeg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yzmmxeqv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ofdacnhc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hjxlbeiq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rxukwiia.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tksrgnkg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3urdhvhgm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fmkeyntr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qhadkztt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pxmtalkl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tayfkamo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vqnkvgpf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vonhymjx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvnpvztn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3altapogl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ufgidlxs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gncnlqxj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bitugger.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qmzvdjwb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3utcizmlo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xxmcsmsv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zexzfkbn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3clavwelg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbsbena.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vhlulctl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aeobhcnz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gggnufzp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zgvudaae.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dxbveged.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3etqeaixb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ympsxozr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uviaglme.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sbocybwb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfflpueo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vizyivmp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ltnxokfx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mkyvoebu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kduxshfm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jnrbyjnd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjhbrqag.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ikjihpyu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qlnhbusb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rysqxgqh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fkjmtqiy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3doqhjncm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gwouxmwj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ramcvgze.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3janrrzqt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qcajxshm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sqahqgia.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ohibnjzl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ybnixgxe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ijkyrxdx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qejrunmf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3penrvjel.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vffleklq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yosbpdzo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qnppgsdc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qykuplxo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hpgobiru.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3esydwfbe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fwzwafap.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xpqfqfiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwllwdon.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qxglcqvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvpvghjk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjisvuti.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gqugnsdo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iuctxwpf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wvdghlfs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ssvakxlt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qlsrccua.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3msbxmpdm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lohfdebb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hcmcfdaa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jryckden.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jqaemsfj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hismhvpp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hsntyuyb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ynowfptr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pdaxgqhh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tzsjlvqy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cctcynlj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnvbykax.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cnmqyzal.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hvnvifec.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pzlweofz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rxmdhlyy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fhnvcggy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mumaxxlx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ienpfxvm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3esgzpvgq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gouenlhv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3taoqzuqb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3egsihawr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jrtihwdg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nfqdhehc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ghcdlrxj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fdczsbud.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oovisnew.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pxgjedda.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hyvqujez.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3njnvkrnu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xkfkpife.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hxogsapy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yilultmi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byckpxfd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ekptircv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3asnjkylf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntaasnoi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vflbiobp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qirsedjy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igcitkmp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3frdhoope.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ghzqydiz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mundbrxw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pldmandw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpytthtj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qatxfuxw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eidptnhw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hbhiduzw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lgivjpsq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xidyfcwp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dxdhbuya.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yajdsdlv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3siyabbws.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdihfze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hqopclkh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lvvmkohd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rivbgaac.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ycjkeudu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gquiipjv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3thclrbas.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xrqdmtxd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bznmcxxw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dfloqyry.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pkarktpn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xjgpdfyl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3efnngakk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgvcamln.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbszwfzz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lavacxxd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bfogpdhy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hwduucaz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3nqycxwbw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqfcvxcv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wxkdwrbl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iipldngi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhjxgho.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hgclfulq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkjznngj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uyhuuxrm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3oabyzbdt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stjbwypg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytltnslw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abbnindd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ihvfikwx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3giaqldwl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apxfshwz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omfihokx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajdeianx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kultuvvk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3edyjrbpg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayyemkyx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uihkdetg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3aspzvdwc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbqjptl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rboqnqmz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3djiqldyb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xuwpaxql.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hukhohdu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bkjpnhcy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3eqeenwmm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wihsdxvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxvtxdnr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zltdyzuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twrultkw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yczuwruj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3drfmpkkp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hxtigkfd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hmojvgsn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zqjwguxg.html


<!-- 参考信息 -->