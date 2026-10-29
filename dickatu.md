代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/ggynichov.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gjlaecbno.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gdusmeohf.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gjojmlbid.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/ginhepabd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gjekpsemh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/ggyiehbxh.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gtbjeohva.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gqyzatsgf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpsiugmic.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gozmejmjl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gtplwwmpr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gcsfflhet.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gmnimdtzh.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/grqjqyucn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gsitycnco.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gifqfwqbu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/geyzkbily.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gntazhafs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grotdjyhl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/girxtpghm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/godvnttoi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/glrudmhzi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gjcozfpwu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gedtjyetb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gnabwmfik.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gfmfjufur.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gwugbiipi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gldmvuqkr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gyyohzwgv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/ggxapkely.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gztkurvat.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gfwzvtcwz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gelsbmpjp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gheubeype.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/goqogdgjv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gnfsyocqo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvlarukas.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gksrmgdud.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gzqrwgmil.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjffdjzb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gkbslrzcz.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvugmzcgw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gxyaznnnp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqghegtrq.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gssvwheec.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/genuugsbr.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gcqgdebpt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gkqfsjxej.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gianwoxyf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gzpyjfshx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gtwaadopa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gugvvfrrp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/giybluvod.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/guqdmpnba.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggyqbobzt.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gmkfmivyl.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gxzcjnoma.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gpllwcmzg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gvisdhhsp.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gponxndwo.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grsvpavlx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gvqngspao.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/goyhzzlgi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gqygzvtia.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gxllyjdxq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gvtmstefs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gadzdxvyj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gejbrpytj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwwnuyjjm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gnbyorahl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gufwmkqor.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gbliiybeg.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gdksimqyg.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gdpetgyon.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gbttgtakc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gfpuouuwl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gblvxjvgi.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/grtcesado.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gragglkba.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/grbpxhvxn.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/giqcfxqsv.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gahczzmmk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gvypizbdu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/grelnjmec.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ghknzlyqh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/glmxbcrqf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/geleurgdk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gsvtkfufn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gijiyvkaz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gjokyemdy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gawpbipzf.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/ggltflcgb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gszremlln.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gfkwprrsa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gifeqoohg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gusuvtpoy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkurdddny.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gbelbkiqu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxgmhgkay.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkpqndhey.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gtkkwnlop.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gzjxnuamf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/grggbitkw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gtscgoago.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gbctbufll.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gxedrxxuc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gemmvahsb.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gqeumjtim.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gqmpsywwu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gjcdxfabk.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gmoajpfmo.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gubtatfor.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gdrrxdltk.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbcazjupo.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gqnvctmyn.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/grmidhhxd.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gwdanyfiq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gzfdtvwfn.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gnpxbhvxz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gbsqzmdqy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/grpzahpss.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/grvyijhuw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gonbanqlq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gajssburb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gubrhyewx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/giloqtvva.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gogmpkctu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/ghuajeego.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gldcedsrs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gcckxoonw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gnezgayys.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdajeurqs.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghexzhqgy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ghamvvgqs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ghfefpvbc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/ghtllopny.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gszobtaoh.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/ghraheopq.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/givelhnch.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gupducfbg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gppicomuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gjhxlmlry.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/galmhhdcu.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gjkexlnix.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gatssncav.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gfhfaekwv.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gkmvgjbmt.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gnmcdzrwt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gkgaeyexn.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gmdbtevdq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gqkmeiwfu.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gkvjfxqfs.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gkfooucst.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gnjhhhtac.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gfbmcpetg.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gnaixxjyt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gsfisvbxk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gryennatb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzhrzamlt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gmrmyqkcg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gcajkcuyu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gxrnpdooo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gshmpffgu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gkbuubesr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gfchodkef.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gacizxbbd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/genamvjks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gsqlmfahp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gwrtjrgdy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gebybtbjz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gtxugmfov.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/glhwnkafz.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gpamtrojt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gflaypdvu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gmphnfsau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/ggjoiiqae.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/ghvwdbpns.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gqlrcbnbo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gtkughwlk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gynsxknpc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gyzgsvgkd.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gxfnrqxyd.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gdrmghypu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gkfirbnjm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gyziksufc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gktdcwfqt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gecygxyrb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gionxjtwu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gcivzzcel.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/guaixaxkp.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gglzhpswr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gwduczrbt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gxexhcxwl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/giypabvpi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gevrfaboc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gsdsdakgf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gcdyqoljs.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gsuaxaxmy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gtwtikqpf.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gnaqmsyqm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gcmuadlkw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gyhgyfuze.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxkgynkuu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gryijnljb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbewsbhot.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gpdkjjklk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gtuobchft.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gkdvpuooz.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gjptwxbfr.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gxvaafvgy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gfechrpmr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gyrnlvfnq.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gqlcjwrxd.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gdhzfiwff.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpeufinej.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gkaqugrbj.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gtunvzgyl.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gmgzmtyif.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gxgudwihk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gipufblft.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gtsxbbqdw.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gqoflvold.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gpogzxalo.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gmlmlulxr.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gjgovgrff.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gcavemqto.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gmdvwfnpk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/ghfaeiktw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gigzdehyg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/grrzanazc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gaiirbqwe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gzvmghzbv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/geuvwjweq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gogqyeitr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdoczpbtv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gcwhneecc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gdryvemwr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gozskjooh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gfdgszpfk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gvhmhzgqd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gckmqnryd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gzrwwqwoj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gwxbgxsfj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gpkalyaki.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmmekwkxz.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gpvziffwd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghhywxfxi.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gmjdzzvrr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gjwxcsclo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfuusfqhc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gbcuqkxib.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gosymntbj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gbknybahl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gmsckpnqv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzdxthnnv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggjcsnucq.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gqaglitpm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gtqzzddrb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gphjcskvq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcmrkwyor.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gskgdpyeh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/grnkwpqbu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gxedpjyps.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gzdphoibq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gcjoignwx.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gjmwwjkbv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/grcoohovd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gegxvsjdf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/glscurrei.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/grzkrafzx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gcjwvgsnv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gfbauzydm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gplnifmll.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gcvotmiqj.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/grkzgbzbp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gdykjnaig.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/giqtuflhw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gcthplxev.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/geuvfrcbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gvrhuwppz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghvenfqlu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gkobepbsd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gjhgohkxr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwipurpro.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/grwasxkrw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjunydoxr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxaacmtja.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geeinqfqw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gcxmcbxxq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gsjxrubdi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glpkaygal.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gohzwefif.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gsvimqpwd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjywkcufn.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guqvqvctl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpruqjktj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glcfbioin.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gesjroeak.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxoeykdwt.sHtML


<!-- 参考信息 -->