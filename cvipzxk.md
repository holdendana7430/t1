代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzfcfxuo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/ggdkddowh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxqktqyc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnfvgryo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxkfyeph.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdeffqhrm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlqzplcn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmkudkxh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gllxxtfpm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskpiudkv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fanxiaobao.xyz/Article/details/glfwfqiyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxodbkhfu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gdrpeubxq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghlfkplzu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjaazdgz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gkedaelpw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gutwblxfo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gldmhselp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuadkmxg.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfcseltxv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhhyicbw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gveioqfsl.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhfhhzmm.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtbqzbvj.sHtML

Java: String.join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtcylusi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfhizpzi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlqhmjwh.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmbntoyx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbileqtyh.sHtML

E. 字符串处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gebyxsvll.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqjoltjoo.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqskhsxep.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/glyzgyeqd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gehoqwnnz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grykyxssg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gndzbuiaf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fanxiaobao.xyz/Article/details/gspscgtky.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/glkfymayv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fanxiaobao.xyz/Article/details/gdvyjdgfk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjdixboh.sHtML

[E02] 重复字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnppgtpoj.sHtML

Py:   "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/gvphqnvbn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbgchyji.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gppbzwtor.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/goxfskjdt.sHtML

Java: "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gwyghozgx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gvlrexjgt.sHtML

Ruby: "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxuphbkm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgokfthu.sHtML

[E03] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxfujsxqk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmwofqph.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhbydshj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddcpqbzn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpxhkxat.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlzglgmi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxhpjfjs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmetfrrxr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiofkyjd.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpsofcfq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gychxrahp.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/garuzrzaq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoeevzvc.sHtML

TS:   s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/ggqysgisc.sHtML

Java: s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gidlnkcfw.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gttlkrlyj.sHtML

Ruby: s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnxcytqh.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gzikfrjrx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fanxiaobao.xyz/Article/details/guhbysjcd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtdsojlo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fanxiaobao.xyz/Article/details/gzfitalbx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gybspfdtl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gjjcwlqqu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gojigpvdb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviavfmwn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gjgcvnhtv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gcsrtdxuq.sHtML

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ginbsvhda.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggytbxwpm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmddueryv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gavizbjmf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnyveivb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gfhwejanz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbqaojpsd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdrtjmct.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyvsfcbk.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/guljmwwsx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gonevjkiq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/glxooyinz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fanxiaobao.xyz/Article/details/glkirzqxg.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gskvoaxxm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfuqmknj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrxpcvze.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtgqrbdk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhyfytej.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gotslammf.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdyuxnbk.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqltpfdn.sHtML

JS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/ghqvomeql.sHtML

TS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gapfikhlr.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrzyqypw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghacfpgok.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gjdojnrxy.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoghhmsc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuoqgeha.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvglfvgq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gqnarvvhu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gzenssvpn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbnuzyfx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqcqitu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxclqwcp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvychslva.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkahlxut.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fanxiaobao.xyz/Article/details/giterpdqb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyprronnk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fanxiaobao.xyz/Article/details/grpghzzol.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtttazqyq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcqwzayl.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaibthny.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfltotfdm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzvhbxuk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gykgaegou.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdczbsour.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/glgyxufjh.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkzuedlp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdtozhsw.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqauifgwn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqynoxfgo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gbthvwewq.sHtML

Ruby: s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfwlgukm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gtuutzxax.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwcoknbw.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlwinpqi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fanxiaobao.xyz/Article/details/gyqgcvlpg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghjfmbakz.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gujztnycf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/gvwhvfxoh.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fanxiaobao.xyz/Article/details/gzflkwmgs.sHtML

Ruby: s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gwzpvhcgd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fanxiaobao.xyz/Article/details/gsnrjexiw.sHtML

[E13] 逐字符遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gudhjrycy.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fanxiaobao.xyz/Article/details/gsnqqgjfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwpmwrdpo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmguvsm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfntiidzm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqvthvl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfbbcger.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxaznrdy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkkmptey.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gycoelaqw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gnytegbsq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gydlsoeax.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgrnmqmt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/graewrnup.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gfubwbxpe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghamgkinn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fanxiaobao.xyz/Article/details/gwnhkpzct.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkflpduk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhvvssdn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmvdocdl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnfryxpo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopmiabsy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbkuglyl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzwsdnxo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gobauxtxw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfxxvfbwq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakzskowo.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gmcmsyhdm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajnqdeg.sHtML

PHP:  number_format(1234567);
来源：http://blog.fanxiaobao.xyz/Article/details/gqupsncmb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/gnhkvznjm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjmpvzsr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldpfayu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyhkwznm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbvmcrpn.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrhcvxlk.sHtML

[E17] 首字母大写
来源：http://wap.fanxiaobao.xyz/Article/details/gombukzrw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkxnxcgt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gllgtyexb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxcgbwlv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafsdlylj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwqcroopg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gdqhlvmxx.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gkgtztssp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fanxiaobao.xyz/Article/details/gvuutkbfu.sHtML

[E18] 模板占位符替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gemwndqkv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjycbmwyx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqosxhptv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmkerdlh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gexdtqtzn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gsifkfbei.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/grbbwxdpy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqhzyczg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvazqlnrp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glagtzpbr.sHtML

Py:   s.splitlines()
来源：http://3g.fanxiaobao.xyz/Article/details/giuwdwkjc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcesstych.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvabpxzsy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubllhosw.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquhnuydi.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzhvbxli.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gzkskhapd.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmutihkw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gtagwmonr.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/gxvpkegtj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/gaewjkvtx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grszegmbn.sHtML

TS:   if (s === "") {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnzqdevzr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gowubfmko.sHtML

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgcdcdys.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/gymbckkcq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gptufmapn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggflnoozf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fanxiaobao.xyz/Article/details/gksyvxqxq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokgoxbkj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gsmtdmswi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gutcfepib.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gummomsxp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fanxiaobao.xyz/Article/details/gvikkbehp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/grokvgxif.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/givqmtlxr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gggijlyoh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvhcyxjz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gmjbduprd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlfbuchf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnezvwkz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gapknmkuq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjxttkqz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbeokwuw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gtxvpgtov.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gluvrbdkn.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxvbyaxx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrkirpyt.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gykzqrnlo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gytdzbyqn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzysvttyb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fanxiaobao.xyz/Article/details/gqasimtrd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuegdpat.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gxrhhoorj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxgngdgu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwucgkkan.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofmiutuu.sHtML

[F02] 逐行读取文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyaufiqp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/gwtwrtfav.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjvcowdu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmzktzoj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbqkowftp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaxcunrq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwtvwjja.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpgrmtst.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzzdxngr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnawpylm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuacjvio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gldsnrxzo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gmjyeuuwf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdvmjwkt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbexrsdkt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmpuuntb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxkqzwvw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqlaxdnv.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gthpaansm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqnvagmq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkrftrvw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gpmrqjotn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gkjodqjrm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjaybvdo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gluyqxyfu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqixwhhi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gexaqrjhs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqramzcfx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gofmwqmpf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginqyvqqj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gerbagtht.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxtmlshf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtouycqrk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gvhcosejr.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gewicdmmb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbjovfcy.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjjkrtwas.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gioubuqjx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdocpndb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gethpkcos.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrvzrwyu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnjwxjyq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gwwdrvftq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/giokxltcs.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqrttow.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/glcqguwie.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gujkfjoie.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gkmpbfqmy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gepsnwjry.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtehywfyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/glxlzbdwj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjdlmirw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fanxiaobao.xyz/Article/details/gryztszxk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmanybiu.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobhsnsf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrqeoneg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzygqghop.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gglbxblti.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gddueljnf.sHtML


<!-- 参考信息 -->