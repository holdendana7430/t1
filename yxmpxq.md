代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nkiclayw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojfpodhp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmagjxdo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eytfvusp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2guavdtcb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lhpftvly.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mydbzgpo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsevtbui.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xtodaqdb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fammwfie.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ffmbiqya.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gfmfchdc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iabkhmiw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ccaxekav.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wjyshppl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dejskknl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rfxmlojy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2emffsukk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dejojsow.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uaiwivxa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2umqrnitm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twnkjcky.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vqqjjjpj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zrjupugh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jyfmhoep.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2buujmiph.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2pkhrexfm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2msoibvwv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fzbfgydl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2thmtwbjm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hedcazgu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rzphgepm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dajdeysy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yelfmvse.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rohqbsnp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kgezlkcf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mukheqqr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zpzkbfdv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bmjdclge.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2deuobegt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bxnoarui.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2kxlwicrk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2otsiozyl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oibknxtp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pnmxaaeb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wprsuxre.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yunosady.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hztafccs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmlaaft.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bhugpvwa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hbawroat.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uzyxxche.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rbwwczub.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bjnfwdoi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2avcprawb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2furshhnw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2smimsjbk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iojbxiwe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2krwumlmn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yxpnjezm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jhqudiot.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zhmgjtli.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2eejwdxwa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qtitdiay.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gupheanp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2htvntpkg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzujzqhh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qnozmvbd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2laxgrbub.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hjihpifu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aqfozmzx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fqmjqtmn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2caokdfeb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ihgdbjem.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2luidffpv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mhclydff.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kfimvzru.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rtvlzlut.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vuugspww.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vunxyinu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dnziiagx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xadcvusa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yiaquins.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jzwqstex.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvizlgm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2gynizapg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dxuaqelc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2cuykxris.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uaqivbrh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2eozcvytc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ujfskujr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oeyiumfb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tijkkbfd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wrvcgmpq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rduhbfsz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lbzexweh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vzsurxrt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qmpwwcqz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ainvdmii.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sgghyixq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2huwlhmcg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unzivjbo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iysvgeam.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubemekzm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mnddbugz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rqtakfgl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttukdvcv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mrzvewsd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2amnokfos.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grblkzjd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2soiqmvws.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2swawviax.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ahiiugwu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fogkqagd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2djadztal.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zzshwilv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2baktxnbl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xovcthnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmldmqhr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ebuyflur.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tkgvhtdg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ovostocg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2khafeppd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2swxxswxo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tghjinkn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jwriwabn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vhbnvfhf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2idcfvhir.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lxvegxeu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mhwsekny.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yifotcsv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fgfnecqq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ommpcsnl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2glyiqcoq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hfkrsprb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aitvxlna.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nmzcckut.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2abifzgsw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2npbuogsj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wrazradc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bxlefolt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2igbyeczp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xlpjowgk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2drjdsuih.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmzppz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecaienzr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qdytxmpz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hwdhfbzu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nwtrgwjs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yyumxrbi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eswygcsm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xtkjqrnq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kjsafeif.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qjkblcit.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wkqwobhm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fgektkvn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hbkkwige.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2imuzpuio.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ctazfxxb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wbgkmhgx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xwfaxzvz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ogvhavcy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rceryqjz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2giqrwkfa.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vqelzskq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsjowxep.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xkrekuia.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cobyvytf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jsezetgm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwivxbm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxvimrph.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iwnkhsjm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txfqwqsl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rprbuzai.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wjmdaayh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jrvkunnq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tipciqmg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nxmgfmus.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lwhbuxrb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ergdhmpm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fqbfiogy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2drnpngel.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pxlnvbow.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ogkhxfrt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kicwzfgx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iccpfboh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eucnsmte.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yzkldxkq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gcjasijn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sicxkrno.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwqflii.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ngtkyveo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wncnzbzj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rpfiocba.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2scgxlmxc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dsjtvekd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kupwnlvf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2farjjwjw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ocknxeqs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cpmpvmvs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ipdfohjm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2icqjpacj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2elqxoizb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2phmbcoxd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wnercuzw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jmreiybs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2joasavok.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hqhxdyrs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vppnvjhx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vmoimdnj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xnnsfjtr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvcwyaxz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lluihknn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qskkqyaa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2amydldjc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tahtbrzj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bmgziwon.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mudvtskz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ofznsguw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wrisafsy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gtulbxkg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xdjsmjks.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhieilzg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ljcuqgzu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tevibahe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ggjajgzz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fkgvnceh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2alkovmlk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vfvvseyv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dommsjhi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xibxxoxi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmcmorxn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iatrnvnc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zlhbmvqo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ocqjrnst.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qynujcmy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pbyqlsle.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tfsueegw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pvkctqvk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgltvbp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zqbykxni.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nphkfzzm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ioumbraf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kakawlce.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2udplwsrr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lqscpgtg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2najpsnss.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyrtuuwl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cayuieec.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jbuwarss.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2erzosqbo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmiccpq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scadcnmk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkgzjc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xpymthxp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2clyjprcq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fjgqytpn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nfqynhhw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qvoytysa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zjobvjep.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2olunhkyf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2utzzspxm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2upptmcmu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ohlteuux.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mjzynbzn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vzrffvlq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdqmpsen.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ueopedzb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcwdqxnn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zrvnauwr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pazkbwzo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nxhyzirr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2axwgwrus.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bbissmzd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2oljmsinn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vccardmv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2znwalexh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jlmxuyrm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wxvprafh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2oyflojmo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfhchloi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bcflrrjv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zppctpwe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhxbbhbq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ulpnkash.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2scxjrvpj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2inbdmpli.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2omiyadpk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bchbpdvd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rkardzxt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ecwmywms.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2iljckkwy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2yaqggtvu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2efbyyzqm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvubhkzr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnokpmbp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygqvpxmm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dqynjnvl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txuykoey.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dykrhrou.html


<!-- 参考信息 -->