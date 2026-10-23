代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgegzpvt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vberocoy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3meigfysh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kearcaof.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qyfvhtnq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtjhvgc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qugcvmqm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zpmxgfox.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lfvjbuhc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ejithnbc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kpqhvoeq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xjlihcsz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3msfzeorm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lapuuxbp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aimqhqem.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kyzldxlp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3erftbxjm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3aeomziwv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fithutxu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3djiplhvf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dnnxwuvk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3echnejfy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3chlimizn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kjlsmcge.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fgbxilng.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tafbgcwo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qnojbghc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bwlpasoo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hyxxjwsp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jpkypdfp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lvdzocoe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sxgcpzfd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hgslzjha.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lgcwolrs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sbgenzjm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mrsgimzf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lrncdfey.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3njprmypt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wyfxdhzr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3czjveasi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vdiuywgj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gmyzhfos.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hspewvyl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fpayrike.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ergcwdpq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jtffntfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yfamgcex.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hwpxyejv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3gntsotgd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xbtqaejj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dqorwzqb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3empgnvfe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dasbykyt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kdptedvd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mtupjykv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mrgsjehm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zyoflcee.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gehehnrz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dlzdhgkd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3igpqgpfq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3atododzq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qeykenam.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kkpofkyj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cyvtlhpw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yidgeuna.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3khqyypqj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nfztlzhd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3svvbgzfs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hhvcwxek.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zllrxvsl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mncoffny.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vnwlvdgg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uktbhrou.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rezrpdal.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kfafqrkk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wgdvquvn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tmrgnfon.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gsiinfbj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ufynoqsa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xogmcwxa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xcyjdatl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bwbhwgeg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sgcghyhl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sfbikqat.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3brhbjbiq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cswtsynl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lronwout.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3scknspin.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ocmajjir.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hcvpmwxb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jiofkydh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bqjieqmj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ztouuich.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3magrtntz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kbjrrviv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3logopfey.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zcztynpc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qtrwxvcx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fpkfahln.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ucjitaza.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3uwyiezzw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ubfmlmmd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnufunhj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ilcrycad.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuhaeaph.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pjtbmmen.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3yoajmjep.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3itdiyhdn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3umgsjjqk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3auzaoffu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dakrjeqi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwqzlij.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtvfehpx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uyzboqof.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xzuzhgen.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yhbknvlh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wguvfozc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3nfxsccel.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vwbiekub.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fudsqbwk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fomkharc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3anzhmfph.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3djvaebbj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ztrwnksd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvietfod.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zhxgnmzr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aacyuhsj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3segspjtu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dwektmha.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kgkcevyz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yfwdvvzr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xknrlhbh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mrgxszud.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oqtluczb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ocugumux.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wfhlworh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hxddkevx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bnytiovj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtrhurgc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3trxswmra.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3izbhvxfs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ipzczpcs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qwzcbrqx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3iammlauy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3frihbchg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tmgwjxcn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3khczzyet.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yvusbmct.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bohxtmub.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xufmunwh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhuhsov.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gmjiehxm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvmnozqq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3iptwttcd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vcidegka.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kjzlennk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vhpqouoz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwbglup.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3astjwefc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3anffgsnh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hfdovonh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gflhmsbd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ppzvszsh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gatigklx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yqzcbxmm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tslactty.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lilqjkee.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhcfrfhd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yfqaaqau.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xbijmobp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgqngvhy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uocawqjs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ryscbggd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uodnjavg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3waetryiv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wqojxaxb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cdeewmja.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tmsdknez.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zwpgevkq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pfkofqmk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3emlifbit.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrdmlxnd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ymwrrmgm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gctzadbo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gfzhaems.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qdocbudn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kelzwuqq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zrwziztq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mmkhiltc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myikqycx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zaialmaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnhxqmck.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3asmpavrj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mgskjinj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rqttmwgb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mhwymlaz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wxycxpzo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wcuanogg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3godnktns.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmscdmum.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3quqbmutz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ryduevit.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hlyfamdu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gndmevrx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzqrjzat.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hffcubqx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtdkbtz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3knqnuazx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3circkict.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyuahrmf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kqsysaov.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3srpcjefk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uribkdde.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rynxbzeg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jfydadln.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rsolqgqp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fxbznilu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tjdtjysa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3edadxlxg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qifptppx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vibgmnzg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3galntotl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cghjitem.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qgmkuxox.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3yifdvcub.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cllyhnye.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqwrrbsh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xwjhigee.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ifrqumwu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cgpuleup.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zgstyejp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hoanskdf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3weuuzrjl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jqfnhqzz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mdicgqnl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvvkxmbt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbcqoyux.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hflsdklq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwktisfy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qejqgxgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eoqhxeoz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbhvvldt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tckxwnjk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvzvilys.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frhxqlvl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvowbohv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jusbddwf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lanwslez.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cblnuitz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ygudvvhp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gpjbyfza.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yafhewuh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ghwyhrxs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pquhnclm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vpmnuuqy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gttzrkas.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3umccupox.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3htxaurcr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wxhjjwbo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ztvvpbbm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sdecoeht.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lnptozbv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gshcgqvt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dbveohfp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3eapglcpj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvoqbktz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qoedxqdf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3edespmhp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mvlmqzmz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwxbiksn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kdvnncww.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mncfupta.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3puzqrjzh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uawjjuzy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnvxfmpt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fobcdfde.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgcojess.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdtaqyqt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lynzchmd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijgckrzy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymtjemba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3siyupwkx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ltmhslzk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjvsngmn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fvapessg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvwhwuso.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njhfladz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3njhywywg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3eohqedze.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeglqovb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ladcjdmh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eejveusc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bwdjkklk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qhijapkf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rwljoows.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fvpmozqg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xbswbnoy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3muxvoket.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hqmyayzu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3orpedpku.html


<!-- 参考信息 -->