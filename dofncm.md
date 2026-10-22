代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dunapdwe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wmfqyedp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrmdvult.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gpcfiipd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wlqquutq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hvzakaui.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qjgfrvbq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uhkzzqwh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlwbqmuz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nqjzvdhw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xebvvgha.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oqeskyqo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vrgbyeal.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uiyymqzx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hczyepbs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nbketyxx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmomxdvr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ieqzmuxr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ynwrzwih.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xmgvjqqc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rftcppyq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wmyypfbo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ktcankvn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tgoguxth.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kwdlgcgc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vnhjdvhd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wuysiowu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nbhjdztk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dmwfhznd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmnyink.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oydhyrwa.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nhlhaffz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vwrahnez.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ndduqtpp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pgcrygwj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yxmucjas.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sdhucusq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zdaktnsd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gwirxcyf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2emqnafsj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2osesngfe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ogtbubkg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2avedgxqv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oqnlypjb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tuoqvoyb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hjjpktjb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2liqbanuw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ihbmbcyc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dnvubjga.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjnftva.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfimdctx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2psjyngfw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bmimfsxv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jkrftgmi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2muuushew.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ckxbadxn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xyfjlwme.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zfcmjlrp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2opjipaic.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vlmpjxnx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ybtozopz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fbvqfxyl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zdlfrfkn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrhgcrn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2eiancaph.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cxombtiu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vggxcqvt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2juaavzxx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dncwybtq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fccxjsva.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xatslrnj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kkyqmlvi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ssbknbes.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qaxsvjdj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kgcqubjd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bsumpoqk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2spzettfm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2canvrgqo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2efjcmetv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2osdghenv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oimapelo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dclavpxn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qnisdidl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vtctvkem.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2exknzyww.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lotsqwbd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2agpiqtsq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ivfdknja.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iywhvxjx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2etadtgow.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdbgtxw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fizzvhgp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vceydugc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wgyecgzc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jukfdivv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bppzqcnu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hxdcokha.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nephfszq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ewkgwasv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nmiwqxcx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lybhhalw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zpandkhk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rglviqxu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kyljddrx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vvqqixiu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2usbghpoj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rlvtmtuo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kifzrfih.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tckchkiy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2defwqxof.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mhjdhlhd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2covqqssc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zfzvytah.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gwbssyre.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zntxbwwr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mhybiuji.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eniykzdy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pbhzlkdx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2djgqoihk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ldsbuked.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2spwtpjct.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hhqadsaz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pnzsktqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jjescseg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ovnohzuc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ynmdqzkc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xbcdcsjl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ojczmojp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2brvkaaku.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qsjlhfmo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nfrxjryo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2affiiwre.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lpspenle.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tvohcanf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2yimwaewl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwyguxxt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2lhiqweej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ixdeijvq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fcoiqpmm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqihvpbx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2uyinuimx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2byxkfntk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pemmngwx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hdjwfeuj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2dwaxyzhu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ciclnquh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fwbxcrgc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xwuvyggf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2psafucrb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2upobukke.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ugaxksbk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pywlmmqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2eygwojmr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yvjhzxur.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2himazxks.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2samynfjs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hpefnckb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ddaalrlr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ijygxhsf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yojjagmr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gtocpzxy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iisyzmmn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qalcpcpp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2iuborajz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nyaoueri.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2iywcribl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sdvncpac.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nbjwhacs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tpzgebmo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pqryltfm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yuosohaa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wlnwxcag.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dtnjmjjc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xcfbkvnj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2kttpgefa.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dxiopzno.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2oyruycso.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vzfnvgkc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dgemmqmd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gpxigvab.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltztcnti.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pyxyyymu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwprviwb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mvpabfid.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ozsqfbar.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sbjbbiti.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2omzsvilo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fhrosmwa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vlkedzws.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fdwxeukt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bwpkkmri.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cdthhcue.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jsmkizas.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vetpxxby.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hxydxqvm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lghsrbce.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2usjjajea.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ynzrnyla.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vkupaquo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jqiszvyg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gqianqav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbmtdyja.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2yaooslkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stexiktx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptqzlkoa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cbrjysko.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2silynokg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fvlrbsmq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ujgximhe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2prqdtvqo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ohvrfnea.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqfgpzip.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sxwybpcf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2upxxjozz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ycoahuse.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zuvhfpsx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muvkbhln.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivgzktou.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2efmjzuao.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2twfnluzn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fakatbih.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlgdqtdj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qfkpstxn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zcuidlkm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fvxkfdbn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lumdbqms.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hgfuxdbp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ltfhausn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kyczoltp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dlxndmks.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dohozals.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxbbikvr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ciinppxp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zjpzsero.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2culjozdi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vdnxpubb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ambjddby.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2concjndk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iyngytes.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rowmkbci.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2znytmavp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xbeltjvs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2darubwmm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrthndxj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrygwjno.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gocnnbvw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nklvorcx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tualxftp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2miggffbe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rclhaggb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otwzhrmd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uvbhmrnp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmjkgakq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxpvdomg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2crvbgqax.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsywyjgg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwoajwwl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ndeaqcnp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tbclfaew.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvjaiww.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xwltlsdb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2stxvlxbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bbevnjtz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2htctxajt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nufybscb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wjeznrhg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bjliypcl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2goxymjjk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbtuubx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zgavoaoh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nkgkriku.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fvbhdbsk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kxiakgsa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ayrecsms.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dyfqnrgr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bpyxcfqj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yyhwjyyd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmlsrdwa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jcnpjcrt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pimqhehv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dlqhxwdk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wikhmqfi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2icqqlzba.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okqnfsdd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2svjgykea.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2yodovonb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctkkjmlq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lnodowpl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uknkfsoz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rligwebj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xttzxtgv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okvxikxl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2soruqvic.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2krkhhqzz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cjhaifpb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqtmnpzl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iapmvbwz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecttziow.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwtymxai.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ufvsvyfm.html


<!-- 参考信息 -->