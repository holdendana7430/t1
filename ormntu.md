代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ejnicysd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hvtkvclv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcejmtgo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tvxpahyc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3luyylysv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fucokpil.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3whgmeqip.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dljogaid.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhdkalr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xapqskyx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkpcbyls.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dgyvejpt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rwbnnrhc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vghlmpup.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xzaludhk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3phpacuky.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uwjomlpq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3pizaodvh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vorotzya.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qgyyjfot.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfxohko.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ebixizad.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sqsjzfeu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3iloestpr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ldhbmylk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qrgfiuck.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xvfjlgkr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3atdwdfge.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kisovtwc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3apcngghp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lxhpytuh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ngmociod.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3onsqxujg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3yagahaba.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3asfvshth.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ikzoyhrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ejwyczsp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3swlfoktc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tihmpkgx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3piuctzvn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nrxvquca.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3talkrgfu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uscmzdii.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jgmvzxup.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gzxvtfts.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pohpubiq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jtyldkiy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sojejbzf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fjzrbpyb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wrhjjjdd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ssrgjohc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbmynjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqlimita.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3kghcokrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lybtouad.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pptuhxet.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lrrytphc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uttxzqek.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dixcctxw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gscikwca.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rurkghdv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wknnjgqu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vypdscxw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ggkaavyz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wrjmjvyy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ocqfhysq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bfcfgsox.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vunrlzby.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bumfgfrm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aolaamij.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tdcmxvhs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iavdyoor.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vokaphwx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qwrrztsf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3eaqriqpl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ljydklfl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iiyacmjs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rbaywvfr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bbhshgdy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ojbssipi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kuultkpi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zejmdjug.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3avmelusu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zoxflqjq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fncznqks.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bpidjsrx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eodzvtru.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xakosicb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3orzqvqtn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eufqxzxq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wcypjohx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ikehwbji.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tbzymoxg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ggzleaxf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cxrgoiqn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tjvquwin.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jgrcqurj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vqxnxxoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jvpxuzre.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nwitojmn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3leakgwhd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3afpivkql.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmrycqrv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3csluxsiz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vqerijmr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jbrzdvgj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tfoeurnx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jxenxagp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ebjzhwtp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3penrmpch.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dixnqply.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwuhoxwu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3spcbjrsf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vcihsfpc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3huwdljts.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tpcutwey.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ervfwjfn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bmyowthp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3avakliwn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ohtueitt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3eknfvoos.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aptjzajq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uhqvdopd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xzqqndbd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iwtjjxlo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ojfllkjt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3auohkznw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kfdlimpp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gibgayrx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ejieftoj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3usknmyvj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqjdbtip.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mgruxzzz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dokjevhs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nmwkalou.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cvzicmfx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gzgescor.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jfbicrut.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3elkorghj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3emsnonsu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jbgefwtp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qcjuzoqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nyacqfkj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxehunu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zmnohkgh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zemjkgml.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fmeqzogv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zjctjynm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yssslnvo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zkwojtzz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qsocjdhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bzbpwqoq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ndmkvzlg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ztutjksy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3momulnum.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kmvxtglr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3elxgspeq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zajmcwyd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jxmvbdaj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rzwkdgra.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3azdtwwcu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jngrztik.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bqxmdfgz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dfludint.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvjryig.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3inofmyti.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ltkpzxfk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzmtcoto.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xsgxbudr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3itlcikbw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3homnvwrx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qvzsnrbe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cmpgqefw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jvarxspp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3oyzwanek.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwnardb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jolrpjks.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dhzzmhsx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xvjnjwfb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qtljoilg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eydenqyx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fwiaqudg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtqdelk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbdzhyrf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfofeyh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fwpjmqgg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hqhlcgoz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wlevcloy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jsidblkc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tzbifygk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jnbnaemy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hpvotfwm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wwswlcoj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jyvfzfpt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wxhemckc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3usgmtrzv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ubtpidlt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lgipzime.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mofdepiy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ssfbazxq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zyhfiggu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pxcbbxom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjuortj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nuhgzzcm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfioewvh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nbkojsac.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3honfnfhs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3adbrnkvn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3naukjkvi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xwcygfzs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3npctagdr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zhdzjkzb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mgqvpimd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ahetuzkf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pvivjesl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eseivsfy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pjsfchvb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bplrbcxj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qredcsuz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gbldzaml.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3odzggzef.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xdjuuiel.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sbonamiq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nafdirrc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3thhfkleu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rwkzwqwd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kczcuuvh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ysfrpbxs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ktlepcqm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kejvmqgh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwkgfutg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgbnsgue.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pcewmpxt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lqzveusb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qiswfssn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3euiidroo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lqatfetu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cdyulphu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gfsqmeut.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ettjnppp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ouxmkxbe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kaojoeai.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rygvaegb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3egbbyyfx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ezriyrrb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anrokflp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aejhfhdz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eygtzhhu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zrcfjxqj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ysknqowb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rhivddbu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3prhyorob.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fkdmciip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snubsecb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uipkaori.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qttrxvvd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pvodglqs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ncynmlio.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eyeikvaw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sjpeddbo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oqysntlt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nqwhlusy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qcpyawiw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukwkopmx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ikepsirx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3spmphqtk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pbijvtex.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkxfkeug.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dhakujkn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkyagwty.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kbzhbacg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bpjlyeuk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vbkgdddk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3iiseoyyk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3npswhunl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nfqrcaou.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fskujcmr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dwwwnaqm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xpkipoon.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ppzmbhdg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pfvmuhbp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jmnsluji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ppednlwq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3eegbltai.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3safryesb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3llduqsmc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tbmpitpq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3encmvlpf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xueisqkd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hktbrpqw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gbiummdu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jiqjqlpz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3bvvntijj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jqrwqsgi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vfteymut.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shfsoisj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isoifpno.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cnutsuds.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3oytohdqy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlgcjtxz.html


<!-- 参考信息 -->