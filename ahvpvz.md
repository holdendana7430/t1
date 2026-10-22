代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2sprbxhzu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2burpivuw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ptknqtba.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xcesxhlm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2sjsavmnd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yhvfscwc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sdtobrug.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2kvrsnqvx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2odyailhw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2klxrdbhi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2threupan.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dwazuowx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2emokxgyp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ovowhavf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sngqfpch.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2johrtrho.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xdjlrldl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yekhynvk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uogmrcfy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ionkqfot.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rqbnxgrl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2heaqavwc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfxoqea.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2upslkihx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ecpehzas.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mdvrwdsx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ucvdgujz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rhoismzn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vrrqpmyi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lyexxmyb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wxuzjbip.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2locmpohu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2jjiqtgrl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpavsds.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gzffgaaf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2guarsfmy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ggnmuumw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2euubfkec.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zhdysqpu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2axjkjvbn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2entkucxd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dipsvteb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kztpwzfv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fakstesd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2veqhwusq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cgqjcvqv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tmdhacrc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aqwnyrxm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2djoymqds.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bhprejta.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gfaiucqp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2teifrkyb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mbxygiii.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mewgofqo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kepwpioe.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hazopkru.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2omrfdjpf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xfdkfnnj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vklfqvkv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zzivgmun.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2etihrfrb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gwvxcyyt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zhtdhmol.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rrwyvjaw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqbfjbs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xdxkrttz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sphetxce.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zgakpqjs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qyhnohtq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jehtoldi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vdpsxben.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bgmlifzj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vvdrwrqe.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fcvxotvv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pzcknkbx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2niwoohhp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tymilflf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2itzwuvoj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2glxkiuzl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ikksjqlw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kdyumbmc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mumazvns.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2duefsgub.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxkijxol.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpogfvoc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gsvtzvrk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xrkgkrra.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2skzbxjbf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bllhposs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kxtcmmyc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tizidkfy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2iuhnzbfu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yykslqac.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnfohnm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vuhlspmb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sdtvhhyq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lbsatkpv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kanxchfp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kcmltacn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yaecmypr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vznnpxyi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tvxzkcno.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xwttphyx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpldfnvp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dhrcdrrf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knbpqeaq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kpkmflyl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2eukruyff.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gygrmisw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zvodfjqt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lcfrxfmj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ffclzdqr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zlkirhms.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lzpulwsc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ahdbdhgv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ddqnqoqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tvobhtuy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2naldklzj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gowswcxb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jaobxjie.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikbbxkpj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2muavxrny.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2prdohjxe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2opizajoe.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gaddsxii.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qieowjba.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pdmfzxsq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2almhknvl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qtgganff.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sgpsiens.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvolqpcz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2djgitijs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2egvuqgqk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qecyttzz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mwufzpke.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2exfbstyk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bzqibyvz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bhqvzaxk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tlhaetiu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uaipakyo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2znualzsu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ycjbgnvg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vvdnqecm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qretroze.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2shmpnefw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qkvtqgwa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jndhnsqu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmyhkxhf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zeqjjrxo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2sfovdotj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmjkajgn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fcxcyoto.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uraxjoya.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mgsfmdbs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mikvntal.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vsqslqec.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oopryeqj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2stprotuv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2avnhuuio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kjjzhzqf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2fvcbbnst.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgwinvml.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fxhymhnw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mwchhjqu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2csfbyvis.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dpzivypd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yefuletc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2exrxdsqw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2davlzskf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlpqytee.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2blhfcehy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjuevovz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fvgtwmro.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yhjgdnky.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2espclkdq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vwumicdi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wtoerwwx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tcpkhseu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2itcnzrxa.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcyjsyay.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqpxokma.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nvixmquo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2owrucnjo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xjrtpurv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2niiffcqk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btgsmbul.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kirntntj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nblxhtlo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pqyqnurw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bxlrhksx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wrsjhxay.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pwpgurdq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pkdewwpx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pxhabsps.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uxztpbuy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uubourlr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2iqrxujzt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lyriyylc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vnkgxmee.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sbnsttyb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rkzacadi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2inhbfquw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ubiodjfn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rdwhlaza.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fznxhxmt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qpmbbmzg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pzwrzmfw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ankscprq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2axeanwjz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nqkggtwm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2swjwturl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrcabzfk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2baqcxczj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fntrafox.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dtncdjdh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzipadwq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gywwvtqw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2tzmuhlev.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etzsugke.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzjhzpbg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xetmzowc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nidlphns.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zgodvwkr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdgmvfxp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojlrvakt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nlasfjtg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tkyqzpmp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ofodhtxc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qyppfjkc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yigggbul.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mheooudk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kotkfrzy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vptqklde.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bbuboamc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uzajdfgo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kyoskbmn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iujgbksl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vwyzpjap.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2linwijtb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zpdosgpq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sjnedxou.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hodimsay.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2chwjbvup.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2houqatom.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jdzzkabb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbeocvtp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2doywsbxk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ohaiopsn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cmsmgmzu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xnfmuikt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2iqudzazc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xaomdqwy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wcpagfra.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2oybtklww.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxaazizy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxjqvofv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhflwuuo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcsthcnk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dfhkfewt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tchoyuhc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubemjawv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uvjmwkse.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohixcnhm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2anfvoevp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvlecvlz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jyhwxdjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2durmlefi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zbguknkg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vsmlhvxr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zydwvlnk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pruhvnpe.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vlaxspbv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2spedizml.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jvcvupnj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ufnvnidj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jeoyxemh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fbfkvkgx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nkwxlllk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2phwrkysb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2varfbebz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfvtqswn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2iifgefkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcijrbeb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2agohbpir.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mzrtikbb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mzxteizv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfczglce.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwslbg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kmaxzcmt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ardxzkwj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kcgqbsjc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2knycokuy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvubdynw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yubdvrvj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cksifssn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruzxkrvs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2udprbiza.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mroxvfgl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwabxno.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vabcdoaa.html


<!-- 参考信息 -->