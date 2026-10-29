代发 wailian999

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gkxicmqxc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gdvvoycti.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gwjqduisj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/geyjtdmre.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gzkklgefb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gfdohggaj.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gmtyvzuvd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/ggzarfnfw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gntdnutdo.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gcncrktzf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/ghjidzeoo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gtqxtizxu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxabrldil.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gnmtuplfo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gfvtmzfcc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gbygkcaoz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gigtftopy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gmizxykqv.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gpsqjwvut.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gdfijggbq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gqziaxbpf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gppbfkpnq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gfasnuluf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnttqbdwj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gvndfiqoe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gctlkoiyx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gswgdrvvn.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gxevtnowu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/giyhupecm.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gtitgvkzm.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gkkijlurn.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gbldlppml.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gvorqpagh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/grjbidxrl.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gjvmkcaaf.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gnteiwfcf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpvjhmykn.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gsewovbaf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghopfexib.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/goairupcq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gfshkqnpk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gaqudtuur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/ginmttqyk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gzdeseswh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gxqyyrmcs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/ghbqwvptx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gwhjeftrg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmpnqbjxo.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbnbwoolk.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gcqhsyoty.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gyxfnycsy.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gznsaakid.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gxrueqsqr.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gzxaomhvd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gvolgzosw.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gaipvjbtt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gcbsklqfq.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gdxvtyntk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gaqlivyqe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gbqdsnzpa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/greiknhqq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbpjmamnw.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gqmgngbmp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gcuvrvsit.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gsiaopmiy.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/grxyxntsu.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/geksdciap.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gxcawvcrv.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gyidjrgwt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gjehrssxe.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gwircmbqo.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gwjwmuymr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/ggaziomin.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gltodgvxa.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzzeugixw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gpufdawbg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gdbnjxznp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gsuknayvr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcegesxmr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gdpcunhxp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ghulteqho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gzsgtoutf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/grgujsohs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gdrpwekuh.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gxlzgvqdj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gdzkmxvlt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gynrxftfn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbebbdktr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glogorzgk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghuynaqxk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gpymqiboq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwuvcwead.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghojbgwxi.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gfnziyuuy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/glheexnbk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gpdpkhucr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gwrvmpgfb.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gziaqkizt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/ggktrnzty.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gsgrderva.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gjsktibkl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/ghjqoskff.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/grbmikuoc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrbftcnq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gtgkrlhph.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gkbunthab.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gnwmzixmz.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gqrwzopdx.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/grqwlslar.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtsqbbrcb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gwbrwrmvc.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gbpkdlprm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gfgbgsqra.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gfohwocpt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gqkzjxagf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gidwendzb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gaaaoyatz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gugqrklyd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gbftcfcxg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/ggrbqzrdr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gmlutpqnk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmpwpsjzf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwbhqzn.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gkzuuhggd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/goctgjmym.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ghswgkshd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gyaynaaur.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gkvqxtkyz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gjhboltzq.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gexvfqxhe.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/glyyxhnxy.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gunsdjdxp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gfuhoqgeg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ghyavqlwu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gurokjaer.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gmjwppnqd.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gekmcdbvv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gmcwxmgwd.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gdejjayxm.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/ggrbgwchq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gvbcqemdi.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gmttmbgcl.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gbswztkae.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gyfyqjouv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gcybtwexc.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gcfcqsdht.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gtmuyyjcg.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gsjhsbyeg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/grbgpmltb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/givftdupl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/grrjxrepr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gpawigkzi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gvrwglwlp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/ggksxxmzz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gisgrrbxs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmopuazsp.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/ggwysqmef.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gmewpgaku.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gzdnxuyfv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gauptvzpd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gugopigme.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gsllhmwbw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gaatvqskx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gwgxryzwi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gatkxxqsm.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/ghhbsusqs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gkmjufsxd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gzrczqpad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gxzpgefpf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gkliosetm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gtcbrhcof.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gtmwqxwhq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/givnspbgr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gnlmkihom.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gtubkwzsw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gsboamwid.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gnqcgoefo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gjhwyesor.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gamkrbkiw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gvvbwzvnt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gtrjawkls.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gajtqwhfy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/ggqsqaavg.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/glvttzoeg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gixcjyquc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gclvkpgcu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gckhqbhsj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gdlrdidmg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gbqcurosr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gerbejodu.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gjlqtdaze.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gjgrdbbce.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gkwgofjvk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gfspfiroh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/grrpwjhts.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gqmpjppas.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gdkaopxca.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkrendwtk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gxdkqcpex.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/grmwjqpby.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gxlrzvgmo.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gtpxhjbuk.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/ghglavffp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzfgbajif.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gtyfedkjl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gehjithku.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gwamazhzo.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gzqqmezot.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gmkzdbboe.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gjsixqfbd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gssztaoem.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gpgoqhfzs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gakwflgst.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdbfjplkw.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gpetjqhzi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsocftsdq.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gpraafwxx.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gfessphyv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gzovjcskk.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkqdlgo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gfvsixija.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/grpvmlric.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gclbdylyt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gpwzbcgpb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbcfixaud.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/grvorjbiw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glvmtgxdy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyeuifkas.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gkgboqldk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gzyqlktkq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/glnokfqlo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjwlabsfh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmrkuabfe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gyejltwzd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gtzopgwsy.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gdwuhdark.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gbrfhebew.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpmavtzix.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gugfucmmt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxeokrmdm.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/glcdruome.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gocufwhua.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guqzqpzlt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gtqakpmhn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ggyjznuuy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gghplystr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/ggzuhgvlp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gapwbzlkj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvlitdawe.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gbumshmjs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gfalvkfvb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gkaqtlbjc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gaxqmjjkm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ggqrowxaw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gheewrsnp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/geepnalhn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gmnureufv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gporjdrjo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gihpbpyti.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gaqcbgxyy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gviifhklk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gszihpxwv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/ggnrzjtra.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gelpuipjm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/glwnmrwmr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gevyygxel.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/govkbisvy.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/ggxcgibpz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ggngairqs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gzramwozl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gdgndrykm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gzclkkxco.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gybeldqno.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gdtqbylnz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gajokvdok.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gqbseihko.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gcgfpxwxx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gjadjwfym.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvkrxitsf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpfzhlhpv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpmnnmutl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtbhcaoch.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gzhfhnpfo.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gleaxsiqp.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjdamfayv.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gnkzyyoco.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnwsvheru.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gggwviiof.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfyrubsxr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyzcxygqk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnbqeetxm.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gljnkycdt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmyylbnsx.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjuzwzdsh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gqwekpuou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gyxrrixju.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gysduvjhb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/grwkbkjpt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gcpvmlaht.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/grcsglkwj.sHtML


<!-- 参考信息 -->