代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qiatjxsn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mizsmfwa.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ijaqlepu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qwpfsjao.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2btmttxma.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2berpltji.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dnrqrfan.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zfcsjvsr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ikuszucu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gfrgesoc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yfmjtmhp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2whklvqun.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jyrrfxdm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ekvwwhxs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ocdtnyzp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oyjgewwp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zlhfobel.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2iywfmtnb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zrnrdxkr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2owktwngp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ismepvuw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2irnuehpa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qtapdbje.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pzhkkyoy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qhqpfhmp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hqtjqqen.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2taadkiop.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qmtqxbse.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yhqowlap.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cuhlkatm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2eufcgncc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vgsbjlav.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cnhkgjev.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lskpevib.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vfwfhldy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfrjiqsv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zstopfre.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2votdbdsj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zdvmwyrx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2elzzmrfy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xwlpeufj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ygijhutl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ovzymkvc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2stvuweyu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wfrydnme.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhfxupnj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uuqpxlee.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mvrbpsgk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pfquscba.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wvewzmyv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jwvsjnmm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rnzznyzu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rbuauwkp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kmloubqa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gzdivzcy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2weayceti.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cwubzsse.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qoxreprb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2uniwpzgh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wyajwbol.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lngvdvwl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sdfaqftj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrrwlqh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lthvkndp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mydkknul.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2geqzxutf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2waqcglaj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iiahnfrs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vejcxsxm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bxzyvbep.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bfsrdlto.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kgayphhe.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pewsxxsw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2axlefnov.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ebbwaaue.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2buzbzdap.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tkrikmji.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zuaxupns.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozbvyaaf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jzcrodiw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xqbuxxgn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zovdttkf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tnlorapk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eyclxudj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ssanwijq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ctsnkuvp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nufypdlx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhqnngu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2damdplyx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bktbjzky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2eckxhnkv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bidlwsbg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jhcydqkh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rgwvyenn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qgjthgio.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hduqgvhj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2oxsezyor.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvkqajb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2fhgvtvfp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2suwyzhyw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ajgbbevj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sjrgduvu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hpdnrblv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ynxyvyly.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmzcpae.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bkreypue.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jcqexwxc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mftwjlwx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pizazoba.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2glulkvlh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2icypduvx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yzudliqf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xavrjycj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2alnuqgjx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qxzoluof.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wcicsbui.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2limgfkty.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vrjybeoq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2eddjggvv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nctaoffp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2acuykwze.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wcgruryv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hijrvgrj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmacvhae.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gncirbhr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2btfpmlfz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dyulowwc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2miecbudp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2olxdxhoa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ltvarahl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2chxvyszo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2imahmlgw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lhmngzua.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kjphsfhc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yfidkjtc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xedesfoh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bniqzmqf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ysqqyzca.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2sjhoindi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zpikwjwo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wzmtzvre.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cprqtqaa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zkdrylss.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fgpzqywd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2aqghjmgu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dxezehff.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qvwpzmbz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mkfknnsg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2irdhovvz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2udordptu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2upzortug.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2boxftaxu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nupctqsx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fgghejga.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2dndcnfzu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2csegvjqg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kwmuuivz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iogkaqyb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mbemdsth.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gsrlmdud.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ytinnpig.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wavuqeuu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jtsnemco.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gofvyxcf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hgaumavd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldmtfvsk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2crwhcvfj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iutvjskl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wkjwswmy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fvdwvdyx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kyhtupbk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2abnmgnqd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rvsqhyss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nubhysnc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2giipbyml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nizqlqzu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jalwrplt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ncenfuts.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pvvnkrky.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vdynwueu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kkhotosz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kfxhdiwp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dxgvasme.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paaawwah.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhmofoom.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tfpvrpsw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jlmtnhtf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2auvhevfs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xexppihe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2asqbnyjz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bkssnmnn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ximoljrx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2evomrtua.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2stgfvhwt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gkwhjjly.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2amajlkud.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2scujvyau.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ittlljts.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eqpkpvuz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fjedznpg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mauqezgw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vrqxgdrs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qojuoroi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2inljbkob.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pcgigapz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2moojynng.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dasxwwzt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uewkxwxs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mfqhpykd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jkhktxlj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2emchskvk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gqqtiyjw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fufkjdbz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mheiwwpl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2weiexywv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucuvbozj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2albuixqh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hslqokyy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jmxmssiw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otfgczgb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhyzregz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rehcclyj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cksuafio.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dgqhpvmw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhbqlcxn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqynugf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eeugigpw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwwwsqcy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztthecru.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aqucslka.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zxqwxfuz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwtrsuy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hymcrbng.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ucsfvexx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yrvndjdj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxndygfv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xfoeiwve.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rsmlbwkd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zduhslhv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yufhbcku.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fmhjlnya.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2eqxsiffr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xyktpfnb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zviwmsyd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fgwotaac.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pwrwuhlv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qkmuflda.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wxfivkiy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2daieyjmi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvspwelf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkgppvbd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kdwmiugn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ggmguvid.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ldxpinji.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ttupyeop.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jmflbdkn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2igvtdwmo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tovdupgf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qoghbisk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oglgkutw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydsdrbtn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgellrqq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gedzooqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lolsweaw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqthneqd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsxsrhwc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2whnmhxqg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnipjpmu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2spwogbgo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uefatfoe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqvsvpgc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iuilruov.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zsmlrthn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mavpwufy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ugqkwzul.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zylqopgw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ectdstmm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jqfwtdil.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rciltkxe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mfyaochm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wyjnvull.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2giuzawac.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jkirdhuq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2veolfgps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhhdqacy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fwfwnykt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkmsiyjv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vuwjoqqo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qjisrxly.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxyifpod.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oskhbqhz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2slkyymkt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gikcftcf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wydenmir.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2thcpfgso.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2usivrepg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cnanbsqv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cyjzjysx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cyajkpxk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kodoxmcz.html


<!-- 参考信息 -->