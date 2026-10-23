代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nqcjsltx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gheqqpqb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hloouory.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pdmljapj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zxwwdsma.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3agnxilbp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3npnqoqpb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ovaogxxj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xypcyouz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tyygrpqp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hepyibky.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3oqelhnit.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vmobcubf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3azjisbdt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pcgsvzhu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dwvhwkrq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rjdeglbr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iuuwhydy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3diewdnvh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kljrcfbd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xeoxedlg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3txsfthlx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyytrgj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qrnjwftn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rutpadsf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3owugfpct.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xcrvorgd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tjhkhgdv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3znzltvra.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ewnnwfzk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bzsyocdr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xedfxfnk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3smdviiys.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kznmkciu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zswtyyje.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3toqtzjcg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hqayabpj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pxvklmyn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3clqqcorp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bxtshmlh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3eljfpdep.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3seefgarn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kkudieec.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ocminffa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qoitybyi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mahsscez.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehyxvwdt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dushqvpl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tvzoppoj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3baujgmdh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rgjghpdt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qaegnmbs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ugngsxqv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jutvutql.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wpfxcoqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gbistsaq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3eyuxunsb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjrioyn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xoqwhnlj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dorseyzs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pxdswloy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtxswbhm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cnbwmvkk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3svqvmokn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nyueqxqk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kklzczlo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oznygfje.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vhozyfav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfrhpvhq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pmekfhqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtgrbvor.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajgvjegc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3euqlhyoz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3njkwnclb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eikgjhqs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ylbegiqz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mqosgjks.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3dgajyfhs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mczfvzuu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hpgzmuds.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hpoiquwo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rdmydmir.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3stcmrgsa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fiallgsi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oberatvo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfkumtjn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpguyrf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mdnvdevk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3igyqukcd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zrnzvxfz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jejrrytd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rvncdzvk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3twamwgbs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ccedrmzy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zfrvoukx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xukfuhxb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ggnlgzyc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3chsurjij.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3etaxbsrt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tnwttfuj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3trgiwhgd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nboadabr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3htfedurs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bhinyqjl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3phqnmeol.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3odctzqst.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ywszpkbu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3scaeezqm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bharbwdk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mbabgexx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3libwnmrh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xorkeakc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ichzylby.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zekwcwqe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ecxptvbw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oowexlcq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rfshsbzo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3omuvsebt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nduxdbdt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qpzwucsq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xeqoqyie.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mscaflog.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkczhhd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ebsmvnca.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tsftbzvk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3feccgmcs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3grmzlsvl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tvheuxko.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3irdkgdoe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gzytchpg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3umfjwcvq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kcziyrer.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3efgblbua.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lcutaffd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dgzuiyig.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hrvrakqw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3huxgdklx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dakwmoyc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3apqobggu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jrmcrdwq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3asgrtqie.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jaswvyph.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ncgdtohd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qqzslplt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ycyijahg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gypsgijg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3oqhrwfru.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lzejdfky.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tgqyexmk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kpxhotmv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kvsjqdar.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3itlhdmxf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ysnkgias.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lwzriqxu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vbfekvxx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yzxmgtym.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uzprebdy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tuypbidj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ipflxxnw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kkyjkpqj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3aygsetft.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zhesjvhe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nudrhujj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qmgphqsy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ogqbilpi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oyuoepdk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3glwpfjrz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3boqnwkxv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lcbzaqsg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ejmoqwge.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vbtvxlra.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ezbefoih.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kepryuha.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mrdvcspm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xdqrixwy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pswfkmgy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ieeliagy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xcyudcpx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vwuuoocs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rvqgeufh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pmtcdccl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ffalpadn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3steklivf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xnqikwfx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3svvxzatr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hpfbpded.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ypabefwo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3orkzquyf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3nyviyeyk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zoljpwat.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjpbhhjv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3msfjdmgi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ogdieqxt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsxjjdd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3amuetmhd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ivbsozeu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mgijygnl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3alassnwr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3oatzdzut.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugxuvpxf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvaqwkxw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iojrxdcj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mnpyanws.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3dxninbgz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3acfpndlb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txkoiiyk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hihtqeqx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lsexdgio.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3osbiutxt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3paebogws.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wtpacbuj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fmfzbjku.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gislcufl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qknzjtus.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qwixnsed.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3kccvhlah.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vvgmzkao.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3klxjiayc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3drlubyjo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuireky.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kgskygnj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eeknxxek.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pxmnbajc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3igbnqjfw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3buuhhmgo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3csnjvurd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3emnwbfjw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvpnugo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3npudenol.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qultceru.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ddrnupcn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqnxvxbd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aoypgdwn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rlxnpuew.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xbuqtclp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kkevvujb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gxfbstzm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vuutnlnu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljdqxmim.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dqdaksnv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fxuytdbe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dsgdzmlo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rofmqane.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jjidzjmv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lljzdakg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gaijubgm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xxoujepv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pupnffkt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ohikmjjj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xqavikyj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nynekgof.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3oibqdowt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jkedqyou.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mriybwwd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pffovvxb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dvfdwfku.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kjthmapu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3symmcmex.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gpkweupm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3efaftaco.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3enmiqwme.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qffthzrx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xprplyun.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xfissmtf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3smytfwwh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3axnhwrot.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3spowruda.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rwgizfnd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vgktzsrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdqzhbpt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kajkghny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntifyokv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkontybd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ekbmawgp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mstavcud.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jlmlqxdi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kbytxwbn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhffzyfd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3magoajps.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3unkpmrza.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfckdlwv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aksplsni.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ywiagmxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvzgbwpc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cfspdksy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3apmepqjp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mgtssniy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yypnfvkn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ijdnmler.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yiternlc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3njwyjlqg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rnvstkvk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nkaugnrn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tmiujlml.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xfejadvk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vcxhsbxj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mjhgpiht.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sptajsvk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3srdtshfp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bwnjoawu.html


<!-- 参考信息 -->