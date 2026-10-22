代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2acnuwnij.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzcclxyr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qenfxkzo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wyeolplj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qmxnahew.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrvvskm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bjcwhlfv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wlpvsogo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qzyxhxuu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rnzapkdb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oexpvoxr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qppelany.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxrdhnaj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nsiswxev.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xkfsezbz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hpuubqup.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gppdnbuu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xudajbhd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fztevlpq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fhwrnegb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mvbrgaqm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2asgvdnhk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hnyqonzl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gxjprpzp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqwxkihb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wnadrkaa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sbweznra.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pccynfry.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mbirzfnu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2emunpfew.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2edvlpfiu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vwahawxx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jshpftta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zjoszydr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tgrojdav.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vzihpgti.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vulgnkwc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlppjclx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ardlcmit.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtkdvpxx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2orqxplvk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jddzpixn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2crruepbo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eubayskt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vhhjmcwu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ufvkdunf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xjlubcqx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vdkagibb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hcwnvpqg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bioeckda.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ryiltqpm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nnmtmtfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxcydlpl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dqwewljk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijmlqafa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bwgoipap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ppvvnwbe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cifslmmn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2trxvbkow.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fdqubbwp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mbqlztjx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tvckojuu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tjvqucpt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cxwecxaj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tjorbflr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pxicdpzp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2txkirtqb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxyyrqg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2blkvjrsy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tcrvybie.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yxbcqvlw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2igemxzsi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mfcmbwrw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rcpmftfq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2prqdgqqu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nbgzybaw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cbilmlkp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yfdsyzwe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kdombwpy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vxocbebs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zdswelgc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfmskfp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mzpdraoe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2swkoyrhp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2timvebfc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ptenvieq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2srqoomvw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbfawp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ftnautto.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2aljxbpls.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hugdbuuc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bvfpwbdd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2awubqiyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dvrncbky.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vqwwzagx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xxqcweud.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gocespud.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2odafnmlx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dhrwfxjs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ipwymprj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2udhzrbpf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nxujyijm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ddizrget.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vgozzzwj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yllhvcmk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zaezlujg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qipkyaca.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2icgbfjqd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ofrfghot.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gfqwqlzc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gaddhaot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhqxkteu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xxqaenam.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpbykvr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ornauyyl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zavxrzpk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yfglxbae.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gvvoupoh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dknersxm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pbazgopq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bhvgtfug.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fvkqyfoz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zkheekil.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mnghseex.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rdsfyfra.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fxlehhmz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cakvgurq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oeyqqcgr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yefrvhfp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwmpmllu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2otljrbqr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cwzldzek.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sbjhtngx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2oyopewli.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pmzvdbes.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2iqdbfxbi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rvrkruhz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cbfkuewn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2aaqcdjyx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ngysfyoz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nefdknkv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ptyecfgd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgshbgh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wwfqtkuj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tfaziboe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fdjzmzwn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wqzzcbhr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqkkyahq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oygvjbwb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2guiooncm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2axlcuemc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pvhydhrk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lupiyudw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2czisajke.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2oktcglku.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2miqoyrsp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2onwsmuzv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rcyodazz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bbetbsgv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2twwcuudb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2yxlebrtd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gfggtpbo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pbpndrum.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2hrercplm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xkasbfzt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieckpjjb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybscreub.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2svvvfgnw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oyomikrw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2psomagjx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mlecxolg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxgqjums.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wnhshpoz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tsiwvgoi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jhezabca.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dwwgjzyl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkjohbye.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2modwwiij.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xobwavlm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kgxwylqv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kmwdiura.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nbizymhm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njdarnqe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ustsynov.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2isqkfnap.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2onqurdks.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jeelebef.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cshxwlgm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ujdvguul.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2feojyolp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ikqjncuu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2muiomywh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dxifmhbc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ckwwewve.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vgnevlhw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eukqyyak.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rahowaay.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fsucfrci.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2htlquyhy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mpycware.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2luwhqyaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ksxyoanb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dxpmnnha.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uswrepmh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2htkyjyei.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mzptjlaq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2czdtvdzf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uethavmj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pqemhgwp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vpxebynq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2iznyolnl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uwxzyezf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fkfkedux.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2edvqqhcy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2snfhnlok.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uaymegno.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gpgohrkn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xuwhkzim.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2csvupval.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vwjifxhc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jvwujyss.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rgypctkp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rbarurzt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kywbkzvq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ittwlkpv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yvowaalz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ewavfjjt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vrurbkfg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rfjlloez.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsdqqhfo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nmzssymk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdrozilq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lyseodsk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lykwhqqw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2sbgpwylz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vkzoealo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2foykzqca.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pogjnvpa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pszhzgbc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xyirbctc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgjwfwwh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dbzaymqi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rwdjlswo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2llbitdwh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lghwiveq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2csxxtvpk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2apksfzsb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2belnbviw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lxyihzge.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sqmyiszg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2srayisxn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jddzmdjp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jwluguos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvfozcno.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2onzommez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prbblawf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2muesbuvg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2juvaaimx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozzkzzez.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ekslxsjx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2htunznxj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ktghryti.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2phiebobw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccfeuwgo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mbzuneoa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jipqhfuw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ytpeyvqd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kopxopqg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rjcmurww.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfknspmd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2obxjbpxq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mhvcffmn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ptyzyapa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fntvshwn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yplaiepo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lmpltxdg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pqlfhfbu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xngswkkc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jcbyfyzl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rtvsaflt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gnjkytta.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tmjnpclk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yoglpccs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zaftqeyx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nvzfujlu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rhltjwvi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mzfkmyxc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2svxcguqy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zjitwuze.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aoctwkky.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zcfqkclc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zhlppjhj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nrkqmhbu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rlnqgdim.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sfgniqsf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjrdbrsu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hutlbnhq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yfrkbupv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjjojlr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yawndkww.html


<!-- 参考信息 -->