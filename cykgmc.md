代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3agikscjd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3achhgngo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rbnidhau.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dfoimoxe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pfxgufdo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tioioswt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hoznrvvz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rmnixnbs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gymocydz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlwvukcx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lsujgxqq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sjfwaoby.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hlycfpjc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oouavinq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fnvhgfra.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gtutipwi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tmuichmj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3fcyptycf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qdylrsyn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nztownqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aaeozyrr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gofihdbd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ublmpguq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3txevxyeb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nxcadigw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jejnwxuw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ebudgqgy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yifcarpw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iiwdkcwh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qgjboipw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qpsazjqv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3semxuhsm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kbykcpkp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cilyhgig.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nebnmoeq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ronmehbb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cbesgjoz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3thmxaslc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vhxnpily.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fjegivsx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjtdvrjs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vegduprv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wdsdoyyr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wchlifde.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lzmuyzgs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3csbiriro.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pjsxehev.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lfbhfhbv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zjxazbau.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3owsoyrpr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oygluaaf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lxakfgeg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3grcejneb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3glonqpec.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ehrjoxep.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mjszpjtq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vayqjaou.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3djnsekrm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uufwhtec.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nffftoyu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qeigfseb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nouvebwz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dzzjwrwe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mfzbbazw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ammhokdz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sgkrucyy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fywmmidb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ltflhcca.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ydcdkleq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xctilzdb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3jmztzrlj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vxmdtwiq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bxuqwtrf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3esgnmkri.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wogocsql.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jnwjyqtr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uetnbkso.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xtbgyrzb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3utcryusz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkeatzml.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vowlxasu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tnojxvyt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bqppiqbc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nhzdyega.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ognzibtu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3itjsfvie.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zrezrgai.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wdrhxkgg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dttwlybe.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3puwfutng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwrvstpl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmvnxgnt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bhjplbzt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oljnvtet.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3huykazfx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ourcfgwc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fhrvrpzx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ghujaeqq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pihzbxph.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wfuhylog.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vuebnyig.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ylqncpik.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hlcduzeh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bkjckwad.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fmtaztqg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3utexdaed.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3owgglous.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fafzfyvl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kfrepmbl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ezmgkuog.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hohmdgue.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwviijdi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nvyolakx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zsmhaiif.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ygjanlsw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qvovmtkf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nhnvdrjs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pxfurfie.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ctvdfdax.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xtleuzwf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jbikzrdh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rssammqq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3opwoqrdf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sgzyrvjs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gcffnkdo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jfnlhacv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3enssnmjz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwycnyjo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rovfhrit.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jxqjqxzc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3heapwljq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vneactsi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yyalitxu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3aguxmsob.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3izdynzcz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3emtnpvkl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3aqbflnqx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qdbnpwnz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3atrxlcpv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ybfkpjdg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qxrsqzem.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kdpfykst.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggcbnfob.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yfpcgxaj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gvhaujee.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3myslhass.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ywasarkz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ofauxbfo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cgimxxfj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pwxoeoxb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3edflbarf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qrnlicac.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lgsrkgkx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3yosfiqid.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rrwjzbrv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ylkpjopl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qhazmebc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3figswnlg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ihmgydyy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hjryhbme.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eshzrdhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqcwcywu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kvqyxric.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmxdqeox.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aebjnaxo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hhjvropz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ridagmjj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bcuurtmj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gnppiwvv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qkwdjjbb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3arqmuxbl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eweulgjf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bsegmgjs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3lgipwarr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ezdwhybo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfrlbylo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrmccoac.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuwslwzf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fpxycvel.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3swezkcmj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyvukfx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqxjldqr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lwctfupc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xqqdwqtt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3towkvmeh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iaffcxkd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dyhbgshu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nrunzfcz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3iswerkrk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ignxejsd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xmzogony.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvhdymlq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vgwfdbbr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zaifivvj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3olbxgcfk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bvevwirr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvswgsb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tnuxiprd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3teqhlaad.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3buwexuvv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tdhnohxl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kduphrrn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3llypwdaq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdnaqvmf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdwjhfal.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wxiryvno.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3opzjjfhb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljxrgaeg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djabacdo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pccxpjla.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkvryjqh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ocxhzisl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypparufk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwjghtly.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kvmcivkv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcmzjoeq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwzqhlas.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3csdcxowm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gxhcuika.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3utvohqak.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gkccssch.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mtfgulkj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fzvykvmo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3xqnqpara.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zjymuyuc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uqfcntdv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vuzutciw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jusdmadp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3norlrvha.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vmtjjkyt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vpqmweea.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tlzglgbh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cchtrbyq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uyclpzqd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pqlonzvu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cdyclrls.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ziclpzlf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqquajqv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijazeqqz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qgmyxehg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3exvziumk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wkvwvzub.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uxzwyryp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3euowhbdm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lixxrwaq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gynhlwee.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nsqzkwuo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sumrgoid.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhkdjoqd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezufplhz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nwwohxai.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trlkfvnc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jcjntlxz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzmquvnp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kuyugdgh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jloksyjd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lapichtj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdeqgypv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugyjiscb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnifprk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wjyqoctq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntewyyuq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fpsadmnu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tidmovup.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bxsngolh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zjuhiqfn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zyszldrl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tfwyxzgy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3llyioztk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pocavfqy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3afrfcnzc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fuxyoopd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzkeolaq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hqbspunb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyfbtldh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xpnciczd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ptrzlrqs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgljvqsy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3opohwzjq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkftzvvj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkppyksr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vfuiifft.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hfdpowpx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpgymusz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rdlneyqs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wytzvgbt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3stozdeok.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcnrafsd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fysiabjb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jamqxqpt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3iikoavcu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fzeoqdct.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sjwyfpnt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3yejeoeqs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xnhviljo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vktdizwz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kiowdkow.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lusdfivt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ceoocrln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3psbmmztx.html


<!-- 参考信息 -->