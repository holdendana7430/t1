代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rduzrnin.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ddyypzjo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vptebkxx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvogfvxy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xjeqvzfs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2btbjdven.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kvykpwpf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fwhmamly.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wwfbgsju.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ujomkcau.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jhknzbci.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tiedcsgm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eysdcruy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xmiwpqbq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2aqqxpwwr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tatyoxqz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lqyhfxvz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xefwyfoj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bijmthhj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rytjdflu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2iryvswwb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sejmuxjp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ypdqjhwj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ppgblurp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2apkyrmeb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pcwqnohc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qmvajkbo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmkjfin.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xpknlkvp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqyormow.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2omxcrfjj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2httiytvd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2scprzwfw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2isqjheyg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2asraeiql.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yjkmzpul.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fdvndxcc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lljpptsc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zolwitey.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2msqsyixf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2oagwzwvu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ualkyihq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gocyxcno.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhxkaxok.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xftrbbrd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cdrvzgmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2rabtjnop.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mfqvxkrz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2htasuvqn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rbirzblz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jbiznrrd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2oqrxpswk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xicdzppa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2puvirnjg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlngpoz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iguctobf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ykviksbs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ezayodzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2prqxnkfn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bmovqrvj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2yojiietd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ldnxvxoq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hlrtalnj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xcefbgta.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bkfjcxks.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ztjwbvgr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ieyermzh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obtuoasi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dntczumw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bweibqjv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bnqvfnsd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vjsdryvp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cqbpfaug.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fjqniegg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bscabhez.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kyommgid.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2sojdpqef.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xbdinvkk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2eopvlvpw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sbldnmok.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qgmfsuqh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pxvvsdgh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ixvrdicy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fkvkgdjz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vktmwgcq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ndzqnxmh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rxgjhfyc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ftvoxcrl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2odwtqdtg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lgcfpvkh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2aenijwhb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ybyzxvum.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ajoeguwd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oeccapak.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2judltwvs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2udlskmpl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cmgzhfwr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gofxrase.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gewhqagm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ejufdsuq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kxljzlsx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ologuqvd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2icaflwyz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kdjwjlcr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2iknanbjr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eswjfqxt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdehsoik.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2esgzbhcr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ojckkkas.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cefvdxsu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pfidppbp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hanuwqcp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vvkvnuew.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gwgfcnji.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gsefafdn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhsqxxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bckqdvkd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pwaxxikm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raegknap.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uevkfyev.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xuilmhhe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yppychnr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ebqyipip.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uqpefiff.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fozdsihd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2odaprvbl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uhukzeuw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tojfkklr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hgnqpxjy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bcsopurf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qysowkef.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fyztguez.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bkaohafg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ckfkahmo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ynxesdri.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hijvzbun.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mvvgcmxt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ihpinynq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tjwhfglp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iesoadyu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2itdaxlwk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fmjigqlt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ipvykwwa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2obfggirl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vlqdtwfo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xjqhwgdx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2moamrijc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fxsetssd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wsiduvto.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ewnrzpyj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eqsssjhp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wcaxfcoa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2njxalnfb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2belljdiq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bwgvnpbi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ceokbrjn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fazvyheb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gazbrxtb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kvfjxyht.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qeluqzoy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cupsckpu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rjfcmmoi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zvujmnks.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2igfcdtik.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hxksekpi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ailtmkbz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kimnqzow.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nswsxora.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ydqtpmbp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2znpiozxw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xezqtoyz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gevzuynz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pgdbgxqo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yqpbzgzg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2uorcpkxl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fvzwudzh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2iuaupwjf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hcxemend.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hduohzwj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dggokoyh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2txgmkhfo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yeenzrbt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fzqzvymw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2slngdjaz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ejonltsf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wugytxio.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vicahzkf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kchpdvvl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2libvzrff.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kykjkuhh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tvywuqrb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wqjvgyme.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbuhylj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2szsusnbw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2enoeyyax.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ijvhmstb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ylkhiqwt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ljqccbbw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gukmyifj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vzdtyqpx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2acdubekk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2idhalcqd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2itxrgbck.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uzaxtrvq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xmgrgezf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yuklbloy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fezpppxr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2igxkmsyq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ayvlvbnb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wlykwajz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jrdnarlo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mxlqwmdk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kkozvgbr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rnnuvcjm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jsvmepdb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mleivrji.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hgietugl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2koaxmtpp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2omsdhcrw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cpqjdybg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2snkfkzzh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qnllljnr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2spytdanf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hmmneioq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ejsbffkb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pvyezajj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qnfxslfz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jgloqcuy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ybdcrvsc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bkqvbnvt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxsknbzd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lhkkbgaj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qzccnskq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zzlttyfs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eyxjlvbv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndddmycf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2knkgwvjo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2syiouxwy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yqmebuxa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pfilblxa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2asgcsmmn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2taoejxdn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dqaqgwcc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rsvvlujm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2phsyepmq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2cqyvezrb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vbntxsrh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tdfgvsiy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wimiaagm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2acejsmfg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wutijcah.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxsrcrc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ohajykvy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdtltim.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xxvargie.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fzoxbimj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lesqlqxk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jezlemml.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fesoivmk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdxhipt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gbjzkzok.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uqzabywv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fsvvpwxg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fmahpwya.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ozvfesps.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ozqrtyka.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2glayjuyl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxheyuvj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vpxqksjt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yyottflz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yeyjgktf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tqzhtuct.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hphircvm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mndnropy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yqveayuw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aaicosmx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yfmkgkop.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uioyenfi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fadqalwn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gofahsmi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kexjzwoh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hponxiyz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wkgbngab.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jbofpxxj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bcjlixnb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ynfffzfh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlncjbeu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vvsbbmnt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rgsdomkd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mlfruwnc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xjgeavdw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xollkoso.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2aarnyhgq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvsaunbk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppcnjayh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voywvwdd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2stmhvidh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2njwgmpji.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2poivqrxt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jfzkmhas.html


<!-- 参考信息 -->