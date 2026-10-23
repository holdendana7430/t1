代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhetomrd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ovkkjcyv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3laqzruyx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3orualweq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ckegfajt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fylvdrbl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xqfnrxll.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wtfefsie.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3neljukur.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tlrocucc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rfukxwsx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hiphkazd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pkcooxyk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3klrqbead.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gdbxrdjk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fgyvnqdu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ctaisbrl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jdhwkvdu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fawlncxf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmyvemkl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tinhezbk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ahvlyvct.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qfxvisnn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uifaxztu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ngfozjqn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3putsdvxx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ezhslqaq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bplajqgx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bgrstfgd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3utlhqwpq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hwmtzade.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lxklrfue.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ouslpnrg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3txkuonds.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mcskxons.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fjhfsxus.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uzlzbeep.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgirupc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3akcmpggj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xhhvxjsn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3opiudnqn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ijikljdo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wkehrsfx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3grotposi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gdsyqgid.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3khgutezd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ypykyyry.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aniwsdkk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fjpdqecc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sjipzihp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3kypzyilc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyocxdwv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dngmxihd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ayizqbup.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tgawiqto.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cmmuzavf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xmadclmo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qnauuqml.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvtuczb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iicdlrym.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3otzbmutd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3trxxwqba.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iwoxoovr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3firulnor.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ankoshej.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3soddorxt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jtoajurk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kexmigtj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qrmnftlj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vybmjeok.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xzuxecqn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hgaklmmq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zejzbpsw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zcfgrybb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zhdffpti.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zcqwoidj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rtsbxwbz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hfdwumdl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3phkrddao.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yodyjulc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bloughvw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ziulereh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hlnqyryn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zgehjlbu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wbuauafm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3skwmflru.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3djrcwedz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aadmhtym.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zaloekep.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qgqrvkym.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jgslcdnn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iaucutof.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dlvluyvs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3srecasmx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sdnpcmsa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mrwqmmnx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bqjtumqp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nzipkbff.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3elwbqljh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bjedxjfi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3okknacdq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3duwjpgnf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tueruhpv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3axsvgaeg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qnjslacz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zzeozqco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3akxlwzfm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3azntvsfo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3spgeldjd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vagamsha.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ojeefqfw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3yveiylxc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3huascvwo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qjgzkvdz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3oqfgmjie.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cqlcazuz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kmewvapa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3sdthmjmi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfncmjep.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmudyxn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mjoaltlt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3idwnzeap.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xngvsqoy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmmvybnp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mechjqqo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3taimjbdx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ecwijlyj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmpymdie.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jhnbmyjh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3irhaxccl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3trkieuhj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pkbopmys.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lzrrkssg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dawulwct.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3cqtoasyz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qdjrimvf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ltltnesx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ngbphbex.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3etfdrqcu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tzzqfsfd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eotaxrgl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dysfljaf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oayqrtgr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3yxdwyvjj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lmtcezmc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3czgsfneu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jwhvgeyj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zdbikyda.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfbforc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dqsarpyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzmaplr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3udmbpsso.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pkdivfvl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bgymsvuo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hszoqrkx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kuxgacvy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xjtbdzoe.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxpbmon.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jreqgvut.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ujimguue.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3oviigxzz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rmndiyqd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jxbsylgm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kwdgplxc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3axahipux.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pkxtcrfm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcrpoxlz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbntfsoj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrwcbdbz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mmpqagqw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xguollne.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rmvieamq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sklmjibd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ghrinwrb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jkaktqjx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sbrrcgju.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wlbidrlt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tbutohrc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iyqyeofu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ypbkzgid.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ajmtjwtd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3sztpiikk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pctcrfzs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3owbvvoyv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hngzhmyg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dhgjfoks.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fnrpufkd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mxyjyggq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3msdnacmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmdmhtwx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yvyyuori.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgvcthtu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmwrkezx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3bsdhjhnx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvmqytvh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gkaxnugl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ooznmjnq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wqioexcv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wryhdfwp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3buzwding.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vlhfgvjq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpkxzifn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xqsmlshq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wqjkxxhu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zdlkhyww.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sjicjfcl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3izdnhzbb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgsadnit.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zkgfhrwq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tdmnmdue.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xwdiywrk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hhtdiqwa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cuzpsqag.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ftcglhze.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gyvaydnp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fhsjxmjq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zcqonzdk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qrnuylch.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3oxxndgjv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3grclfryz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qtfxwdwi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3atraapjg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jsohewag.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tlfmxrsk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ccxzysgt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3djvmgrox.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ansdxnqw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xzmaiqpd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rqrutoex.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3otyaapar.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pgtnpuyv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idzecrqu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbihgoik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3offvgpkx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qyfkgfbg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlsgffka.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwvvqnrm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssevncwh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pthjdbcq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wlhsmvua.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nypdkzvh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffiwqyfm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mzjjjnci.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hedgwwvp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpscfuhd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxwlbvna.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zxueyxmv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3exaepsma.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wcmqmvng.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3npykqxue.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tuvalujn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3avetmuii.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjmlohc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fuwuesfh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hzjuxqbm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yjfdtlpo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3sctuuwjr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dzggyeao.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3glogxpsz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cvlefdpe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3soutqpcu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3louvgdwg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ulmexrwa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ghkyjiuo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sfytzpaz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfwmlcnl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzmvtijf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lyhedscy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cpzwdiul.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mjgrrdjg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vqqyhbeb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otwknrxh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3efpmylsh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ugomroku.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbsjrfgq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uyoatsei.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oymlhrck.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cczfptfc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mnlcotbj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpdzjmfd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmspiebm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etxsryfb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pbmhaxcy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khprpwqe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tvgrxqtg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgbwxtzs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkaxlmlg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sslvqexc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3uhxmnoew.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzrvozal.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jmjvlxxm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mihdqilr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tsjnzail.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3krhdezsj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mgwujrat.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wweqsckk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rnnitbal.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bdtunfqw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xcgigkkz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zclpurga.html


<!-- 参考信息 -->