代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gkacbdlqq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gzchbpzfx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gumomxyhk.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gbibrqvxh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfwmdcdsf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gojzhifsg.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gpuarrcmp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gwdnanzdd.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/grtnuobic.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gzajfqxys.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/glflvrnpu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gwsswbldb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guftxfnlg.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gnolicgwa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtvaczbva.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtuakysey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gvxnjzoje.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gswjrzamz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/goiagdibp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gavvhiojr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gewlsilra.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ghihpdcdz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gotnzxmjr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbsqaeepq.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwqfsxjba.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gssvhyuey.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gtetafllj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gglrzpvrz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gsedivetw.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gvrhknxno.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gvfovxbvh.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gpaeigurn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gjkgrvlzr.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gcndbutgi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gxupfguyn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpevjxnui.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gurzmqqzf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gefcycafe.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gwlorjxxo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gxzltyaxe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gkvbdpgxc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gydfzyuoh.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gbeabccck.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/ghgmzjmaq.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/giqvnaids.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gvrxxhjhd.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gspvlrrkd.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gmbdvmppa.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/giqzkqmkp.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/ghosddehv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gakeuxdpa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gsxiqztko.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/glbvvptqe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gnhhgzzpi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/glebfltdb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gkqmkohvr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gvdmsocll.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/glhctvhwp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gwpdzxdun.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/grcpryrqc.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gagywlxxa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gsmsdngam.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/glqlarnxt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqftwtkiw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkpvjzskt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvfbhzjhm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gtaqeeppy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gusoifngq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/giihbycjq.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gpfttokab.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gzdfauabk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/grhdprwwg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gpfvzgjfj.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gmomcncru.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gipvtotls.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbgzpsxom.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gnqqomref.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gnzybnsna.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gzjzrvfho.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gwkefysrd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gtdharkjo.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gdrfkrzjw.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gpcqrrkdk.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbxwlqgpz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gtlzvbzqf.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gafbyszep.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gucfvzoah.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gwqbnpwmz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/guwsmhqwh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gfpdnoyxq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gcyynlifw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gftftitls.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gtlglnoej.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gjvouveia.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gsvexchee.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gmjdxpdub.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gneynflmk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gmjnelkeh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gtgvdzkuz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gpveorkjb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gbdvgnkfl.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guqrwwpxw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gzvnthyom.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gxovzksfc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gmsgesdci.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/ggcezvhpx.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/glkklioqc.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/grhmhzpbp.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdtlynnza.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gryrvpqmg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gdnowyeff.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/ggcggjpia.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gmyftaeeg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gwdalwizd.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gxcphremr.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gjphkcsgo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gjhnwkzgp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gcwlqejuk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gqvndankg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gxxegbowv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gvpubknzq.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gqcukudqi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gcdnlpycg.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkukecwuw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gocysclcb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gbcgulrks.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gwqkpqiro.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gwzivtokn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/ghvbfzpjq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gfgfzoteu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gsukekoyi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gyhfwynzz.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gmkvevbld.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gwzvyxbax.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gpbmbopqs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gkmqjkphp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gaydvmvuv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gmhdkqiuf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/goowwyjdj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gtwjkmidg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbbwqjqav.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/guedpziqm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gkcaxtwxs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/guuoudrun.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhgqozrj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gvlfgymfx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gxpcfcvkf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gxcpcgnuv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gqbwhqgqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/ggwlwdtei.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gphzpwaqf.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/ghautolpf.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gfmrkpofz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gplkavllp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/giloxfofj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gpdvafhkc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gqebsbjao.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gxugvrofh.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gdovxjmav.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/ggxjylouh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gmwroxtuc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/guravpxmd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/glivbfsst.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gvtotlxzi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/glalzpgdv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gdaiabvex.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gykqnqmjq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/goezxunqz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gtiuludao.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gogclsjvj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gjmfcnjvc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/glvpgcett.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gnxpvsygh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkztfjjuk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/goilrmdyt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/ghlsrlisw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/glspuhvhq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gkmuzoqqf.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/glpopxqdm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gufkkfcjo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gjfewgbca.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gtzwixjue.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gnnwqgwuq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gcgttbxvb.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gzjqbvvjb.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gldzwdpwh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gtzpmcesa.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gtvxxruqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gikfesghn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gimairohn.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gqdfsmioz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyoxuprvi.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gphqcktsc.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gdamthzlt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gsyckahnl.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/guyfztask.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gqymekxqe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gcpemacud.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gntqsbkgg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gwoacalbx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gejuoiahr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gxdobniak.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gcrmmhisr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqstjqnwx.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gkrohnhqt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gmbtbpsex.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gcckgcori.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfbcsecgx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gpgtubkna.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gtorwqtwf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gpyrvhdem.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gylmxesml.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gbqydgmxe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkqwxknxo.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gzdvsjfjr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guhzmqwao.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gpioojjgm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gnziusoge.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbivcynwi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gqtaidpqj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gfyfjhnrn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gdkbbwvvz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gvqjoyoqj.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gontidohi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghvprxuly.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/guxzzuljr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/ghzdgmrth.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gbdcitjxj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gxbctpapv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gruclqxwh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gsbntxzkn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gykbgrafu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gmamvonps.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/ggzbskivf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gnahylydd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gscjyzblg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjmwjngmt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/grzajraoy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gieigvqib.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gpxkmdwma.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gzyaibudc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gsrxeqtxg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gmhkaotcg.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/geznwfgop.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gfujzwnvg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gimfarsgn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gezxqidqj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gadxtvktf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gwddygpoa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gnjuamayb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gfucoelna.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gbsilxacc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gicrrvwby.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/glafefalc.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpoxoopgz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guywymcqr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzqcevxng.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gmxnjmqzo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gdhuveelh.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grkipbmjk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gswqlsfcr.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gyfffcnrk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqpxwpbzy.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gikcysber.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqgvvoqpn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/goyrairfh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gvujnymcc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gazxwtcgu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/geojsbxpk.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdldqdlsc.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gqkwjxojq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gbuazeelt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gembzpiih.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gohomqfgf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gmmezwjqi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gisnsufxp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gntwtrrvt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gnzfofwgt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gijpgqouw.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gchumyrwt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gurdhapwq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gaywabhej.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gjnjayzst.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwdpfkytp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gthkfoonb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqwifqest.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtbwemhfs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gzcwendpi.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gvfvhlwdu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfbtwsllg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsbjdyvxb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gfedkdomo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/glcxwylwc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gsoknxsux.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/ggjrjitfg.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbzbpdwpv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gbkjfyxry.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gbucjtesy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gepyurxgn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkjswikko.sHtML


<!-- 参考信息 -->