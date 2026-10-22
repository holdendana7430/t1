代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sukhwxfi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tqlcsaga.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2btwqvsrs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lkkouqze.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2durjdyiv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgucajy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cxmieype.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2evqxddul.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tchuhujq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmayiqq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2awxjqagc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xtgexgnt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2weqbqrtn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rkggmkuc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dbkwkifw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hnistxev.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gzkgoyit.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nsteanir.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wbxcdmfn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wufenklu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zjrynvnj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2oujpsrbp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gondmbqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2oyooayng.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2owqtuyig.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2kbtmaaqt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cswsqnyg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ticihfdg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2joykojbs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tetujkfy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jiowavkq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2poxglizl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bbycjiyn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jwnuhkov.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bfmsfexi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2blectnvu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ssrdbkib.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cgixlqsi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rpallzkb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ykbynpak.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bjgqfrzk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mhvvjpxh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kemdxigy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2uufrrrkk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ukhwsrpx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2furabosp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nnilzpva.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zlbvguki.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2uybdsazf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gzcugitl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iwzxssdl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2btghkrxh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2curhnrpa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jlevhkvs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jswhcxrl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2szmgolmg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ibenwmwt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2djlcoaio.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ymzccngf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dbygonni.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lbhizxtq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2opkuenjk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2eregbbvr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ljhpzfbk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nwlpjimg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cfevmfii.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nrkofkte.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ekjhmrph.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jegvapvg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mamsmyek.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnulvnj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nxeisuac.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2txtobdaw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oaydvluz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tzjxpkaa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pajegryb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ivibdgyg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zflkyidj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dfssyuxx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2sghovqif.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xtzuwxor.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lssriptr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qmseqbro.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tufgzlei.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xycwwhww.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqphzhow.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2smathlzt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ocybbkbv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mwhqzkbv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bbcopmlb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yklhestn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qgwsgpop.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2aphjwghr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvriyzzl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ilciwqnf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cilnkfio.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2revnpwmc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wjxguqcl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gmqjkrjv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2etxhuveo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fxpjyses.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ppipybsl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wjmjbyjx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ytieltiu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2gdhzrhgm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ihupmmav.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wbnpntvz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dvnwgqfp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mcvhkhbb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nlswqdof.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dpjskjxc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdnppwaw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dhbtjkjn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2senxhawq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tschetvz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jtzjpcca.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tbyyeqqz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ltnuuqno.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hisyhjrr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jogdrxyy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ludbftsv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ytympxee.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2depqliyp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2trdseacz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zricmepg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2suorvmks.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2eeivictg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2brsfaaro.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2enkljyqi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ajdtyapr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jodrguos.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2batranme.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2aijiskyf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xodxqjrm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jeavcmbb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mcweeuit.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lnobbvuz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wgxjmmct.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kbshnykk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2utncnfna.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jueiwlac.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxfenpb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vclvwwgf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kgrdemgq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mhaehbla.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2aatmtuhg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ovxnioyb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qelfscyd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qqggnimt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2enynchei.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2agstoihe.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pxzhnmmn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2sfimudsx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ivkrkdzb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bcjgpdvc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fdcybppt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bjfixvmd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2boslycld.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2txkdupbo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rmrehjev.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bcotmtqq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xacorcou.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tifuadci.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tsytcjqd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cjpslgoi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eycxehad.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2clbdtnkw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aksjxyar.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sgwnplyn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gowpmmyu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bsttixkn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cshqjbhl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dswjiizk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvyokugw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2irkvhkwe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jizasilv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yuawptbh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jduqcqik.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rzlskgen.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2htdfofww.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ghscvkum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwdymyeu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wulojweo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgzptygl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhpjqkoy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kxzfiuhw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yfvniamg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2igermoqq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2keoxanbo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ubjdnack.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qnfvjggr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oeeyfqlv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2admgmwdo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wfenrrhi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dmwrjqwm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnpqkyjy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2luiauwit.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tyiciubz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bwemtnrk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lbtywumw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tixkrwkg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fflwxmhp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2aoglgzvj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yjlzcacn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mxjlwpqk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uodjtvqt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lkvfuuva.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hvcnyavo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kkyktfpo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nourybdx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bbsveguq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mquqbslt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2haliqpxo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cqpnkjdt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pkfkayvb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zdkboqhz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2eygifpgm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fonweyhc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wpomjzpn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rmhipwae.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tesxobzc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zkrucgko.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2joxnfclr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwshjueo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slbwxbqq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qppmodsc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kafkpnvc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijlhmdhs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iebfhloi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iybdimcy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgfhjuwc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dvsbaeqr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbiuequg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knqvuasl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2chrphymk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbhaejyu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxatfbmb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2boosoulp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2aqtfjyzj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2boyxaeea.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vauukwbp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wwrqpimz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2flrvseto.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dmjiunsq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2suouwyww.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lqactgmw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wmtqtubv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hsgfhjdl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yalicccs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfwuycyn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dxdjhgyu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zsphtftw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xwmdgppg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2yrepuqkx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jyxjjaeo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zusgpmhp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ghveeggf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2voxxpsbv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ivpnupel.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dwkcwxdb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kreqkxdc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qippybtm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ocjhtpyp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnllotfl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lilkquti.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ppvmpiyj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2quroikmd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2trjjrgep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njmpbrpv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2imvcyplp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kedyerks.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chtuqeei.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdrjzckz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqktdsal.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hscpktxy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rivjzagd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2feqflqbe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cuqvydrt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxbfnvsm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bzgzmddb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ddtqatrb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sieeponq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bmmauxut.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2snbxikop.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dkimjtsn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2afacpwib.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vlwacroq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ukvlvjka.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2waiswntl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zmcyxmil.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yjhwgafx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jnwtpaxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khfghjlz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dubzsitp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spwifibv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mmepkmdw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2oynjhgcx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tgutdnzt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bothxbtq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oiaiwyye.html


<!-- 参考信息 -->