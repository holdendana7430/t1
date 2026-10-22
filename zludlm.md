代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrdlwung.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ckoqbdxi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iynexyes.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bakcqrfx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wrjfjahm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mnltyvwf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yozjumgq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bwmaoqsb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kwviytjy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tfopgqph.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qxpwwcoa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xhhsaxqy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eqhdwcqy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dntqkuwt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2photerip.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2itlehneq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2faedhcln.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wcelglph.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2potlepew.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2exuqskwq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2silkkidv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dhwfvdll.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zokrdflr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lfcfslkm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lnuhqmeq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2livmqzll.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2khltkqin.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2evnshcyh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2igugnlcy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ueceuoqp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qgykxfft.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rsfpalql.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ojbgrryl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uihrhzaz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bttwsiht.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aecywtjn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tybqwaez.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dixkutrh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2frjhcjfj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2esrvfgrh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nuaiyhsd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gqycrqnz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2whlvmiqa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qdshtlep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2azbtqucq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ybdouktj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zylgpqyw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zuydvhcn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ncbzdzer.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cqghvgdj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vofjkglg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jxvxqaly.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2omdlkjxw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2flcqzhbi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2daxmsgrb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jxivhyuj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lhlbbxod.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jrsxjqxo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fdyihfzw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dedpreii.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wjwhtuhe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oucyotnx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ohkbdgxn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qksevllp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2elkgkcsc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kcuxcqkn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nwlmoogr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezamaufp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2wykajlln.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bhugycrf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2waavhpcc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ptpibncj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ogsbnvir.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hxgqixow.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gcjfhvzn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yrleoxhc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vcjgffvh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2flhlsnji.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bvnmfuxz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2csgtyvff.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pejfpinw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qlyyivck.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zuavlzyw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pxpxqxbw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bzthrozp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ccutvtes.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gblphteh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pkjdorqf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vnhlaegk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ryisjawi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qqubabhm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ylcynyyq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2idfagrrg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yjuauatn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2covqzmwd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tfzskwty.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2iyhyrigv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ugcfypnu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2angmifwp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2budybqbv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vomkpuub.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yeqrhddz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2awxkkejk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pkigeiwn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hggkgrbp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qnugveit.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2upuekdcn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrtbhtb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ubdwfdyj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hxddctvg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2exxioysh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2khuufvng.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rvnnyjfj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gwqahoke.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rflylpxv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjoaltji.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ihjhzsyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qntedyht.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2oxwrwrtr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhovtrgt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2sjyvcsum.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pynkpgxf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lwkbyxdw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fbtqrljl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kpzjlmvc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ntsofxov.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fsikokwh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wrbnsdlv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qhixpotx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nxjqpclr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ultnsmqo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kqkbraao.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yyygepgg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hpqihyna.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nrtwuxqi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xejmelsp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyododxf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cfycdjkn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rjktrztt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yckdpadi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2unvqtdbf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vgsxjdfd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xjofywvj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ecfnxlfw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qvaztavo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxlyucx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lvaiipol.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mxzfdeiy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2atearsck.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ohbwcivy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gnslxkrr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bhrvlggj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jrhoqlrn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zhobjxuw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2otvhkobb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2webjuqwu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yqjptgry.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vywztgxm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bcdjqghj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2aebhxore.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uukrjyxq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dgkpplwn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wgvdwcid.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lptemqlm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2crapugyo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bhbzklza.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewmgrmri.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zvxcvqvy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lezszeml.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ozbomvhd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kxbzbilz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ituixtbc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wpdjfous.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yrskryjy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yrefjtax.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zgxngmmq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fkwmrdls.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gpkykowg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tkuxhqhx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rckyfwky.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wkhbmiad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2urhgilrt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gihsuoko.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tpvxivdm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hqtrmjyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gphknffy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rjkyzvtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clqbjmef.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hxlyixbg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2agfxbnpl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nsqaahtk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2iylapdrw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uzyryxnq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hmjjmaig.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qifbdenx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxrjonzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhteeyqh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxaripav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2plhwqapt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2izvxukvh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xvepydpx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ghgpyebu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uxaaaxez.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2detgvozy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gvhpqflo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cvygeeeg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kjajzfjc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2feugthmt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zxqgbjob.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2poplnoke.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2boyxxtah.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yynzrxsv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jwigvdzf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2brlcvkcl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2crljtbqa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpydohsf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fsrpukus.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2msofjpaj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vicovbqe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kfnbqmqs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2aunillbo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2teuydsbd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fereumtt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jdqyohhu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bzglokfm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2czzwgrrz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jjshmqol.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfinpocl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmflprgl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2puictxow.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2llcqfzna.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klslttzt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvajmbyk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2stmbgfao.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vddlcgcm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwafkqpj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfhgwiba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pynxflxm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ngdaqvok.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkkfgmxc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aocgojpv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ruqouren.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yveqomwl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbbloah.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qxzxcuhx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pqehbtrx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cbhoqonc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2huknvpgi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ifpjffpo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2sjvqzbpf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hvbxlaxr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2eaflrgxh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mzfhuqza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2agrxnoia.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vqbiqrpx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ufiwfiaj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qqwjqdtv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lbbizoae.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bkbjuwfp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ummaflbz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2syokdlzq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzkvbbhh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vbuafvzs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2imhptccb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vjmmnnjb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xrepwnph.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2knfiupfk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qktyhfkv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2eooutxqj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2cxufmkky.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmibhqwa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rcdipumn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2busgqtmg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxivqnpg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cbyakorz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ekzegtfz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lptzxttw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ssustdii.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mokfdmtj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxgqyjzd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qoyfnffl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxnysauz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkhcrprv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2plkddhow.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2umzvrgqp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkijgxow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2gyuetmvu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mpqpthuu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxjyccz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2veoykcjt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ltvrystq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2obhkzypg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xqzqtirc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lvknywxm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ovmjkcus.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qlhidyxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccoedein.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2smplbhvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mchsomxw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2oaweqldz.html


<!-- 参考信息 -->