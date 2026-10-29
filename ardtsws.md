代发 wailian999

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gcqlzcdel.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gnvwpnrkb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gvrzazktf.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gfgkijoia.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gtwprcmzv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gypsplckt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gcckhlync.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gmgmxzrrn.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gofboetyy.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gdjfzivyx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gykcovbjf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdiifsdag.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghckdafms.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gzhixhyhu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gwnbbkjwt.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gurklpkyn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/glzbeihtj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gcxcpukpc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gezhdmhdn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gbehupjel.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gppnepddz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqedleki.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gplelmdwm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gczgelbtr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gqyrvpzrw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gjsdkizrh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/glsxopnat.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/grszxciix.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/giumvvdtf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gsxshgdyc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/ggbjssevt.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/goqoxioyk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gagdmouqb.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gngauetmv.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gexwkpzej.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnafyjbne.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gvisizwwj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gxhtugrfu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/godxsfumi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/giukkdynj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gomkkygcj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gtamvknvi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gssttpmux.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/govrtngli.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gdujtcnko.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gswxlaezu.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gyrlxlqxe.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/ggysdujvp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gzkkffjkt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gtqfbmgoz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gfgbdmlgp.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gxfxofrvq.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gqhgxdnyr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gjwteuobk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gsvvwjngp.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gmydxtchw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/grygqgrlz.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gtugnetdo.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gckawasdo.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gvhzzfbgr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/getlfwrmc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gsrwvzkok.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gqitaiubd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gfmgpngnt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gmfryrvxc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/giuwbeocl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/guirpvlqy.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/ghhntkpbd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gaggfmqfk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gtuhanhfa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gjqrlxusm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gupdopxan.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gzgtkicog.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gsuwudfot.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gvxjpokld.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gpnfuytzl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gwtzhfoxd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gvyvnsreu.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gfaskhyhb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gpbpxepsi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gosmszifv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gfhkinacb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzbumuj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/glrxxxhmd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gfacgtmlc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbgklfbxk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gabivcfpq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/guxbgcdkc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gvwoqyqbb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gnqitfjyd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gvnotumaw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gwrerupah.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gtkwibkvi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gyggqahen.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gziqiktml.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gkvramsaw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/glntqeivu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gbznnjlax.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gplsizvyq.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gglsdublq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gaadvghah.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gjdegcmha.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/glzfxhkke.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gbjqbpqqe.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gyjaqoysy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gzsqtxlbu.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gsuhlflcp.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/ggolttorm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjbibcipk.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/goznjuipg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geajvsjgj.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtwplazjl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/getciwugl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gewmnsqhe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gaphgkvku.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gihwwjjhb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gpravyyhk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/giwhfoqnr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/grarkfusk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/glfxtaqpk.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/goegrqgbv.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gdjswhuaj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gwsjapcwj.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ghqwjpwnw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gumpbguhc.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ghadkwfuy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gmcsiegfs.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gqkdsumed.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/ggffbfsfy.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gyslztksq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gimwcfwtl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwtmikinp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grlcbbigs.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gvqmymray.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gcjhthlnq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gwftzvblq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gattpvfhl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gvmcfcalw.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gzrdcspvu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ggbwzsjnr.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/grmcsycei.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gaszymsuu.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gnavrfqyg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwpisvwub.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gmguvzxzs.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmzztsfsh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/govaufiys.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gpgpxzbyx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpgtkqdmk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gwhjvcpfv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gwezgxazy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gpimtbbsn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gcqtsyjay.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/grvckicrw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/glivtjsbz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtegvkdau.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/glymvezyv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gczyneqil.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gximomjwu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghktkgvdy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkmigxhem.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbrccehnl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gwmivjjsq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzkluxzzj.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gevmazomo.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gfnwpsuyi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/ghmsrxleh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gaijpvwet.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gsupgtipw.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gxtozguva.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gukhqxelm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gnigmsnnq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/ghrgasmfq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/giifvqanx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gmkyfifkq.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/grazxxqia.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/govlhikac.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gqykxueme.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gvnznpyja.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/ghyvppbud.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/grhxwhzbc.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gelhtbhjh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gzoiutvca.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gxluqjabx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gskwbnknj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqkhuaxqr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gawjpgebn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gqokxcswg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gjhzygepf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gkaizeeac.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gsfslskuw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gexjewkgo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gfyxsvnzj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gqmnmuqfu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gttdazwos.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gabukvbtc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glshxqhqn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/goacnatpf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gltlmtnqs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/ggnkreuja.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/goqrwxemz.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gwcrnrtpn.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gturrites.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gyqhbmaaq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gzrirkphq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ggvnajzno.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gsdigwdat.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gjxsguryc.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gnwrkycqz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/goiprimvg.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/glgciqwmu.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gepuwbafq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gbxolljmv.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gbhrclrxi.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gsyevzmjk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gcjujizmt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqakcjhml.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gotnsxgmh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/glrhglifc.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gditzglqb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gsrvuqbtl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gakpfxnzl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gbissgvlw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ggdhiurwy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnmnkqkiw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtakbrbji.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gvckdporj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gvyqanpbk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gdjdnpytd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gcfqttxra.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gvraldkvw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gnggvjjyz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gvcqhdvqy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gsctxhnxt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gfboinwac.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gffhgxagq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gctlrosxo.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/graistpvr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gkhjyjira.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gjwwskjrf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gtdfvbttm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwjaqtyxm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gwpjesiev.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gbfiijapd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gwilqkdfz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gqqgjmtyx.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gcrvluvww.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gewwewytf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gyuitfuyi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gohvjqlpd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gcldhyyfl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gvncpagmo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gkotoixak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/ghhkgqkvv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/ggohgqhyg.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gvfrrbzaf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/glvwsclfn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gbkdnoaje.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gncwxjowm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gzxizffwn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gunrjlfub.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gjudyjuzc.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gnswdmmvb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gtyutodbd.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gxwnbdjdq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gjbdqxkij.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gprhlotot.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/grqjnnqxh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gywvtkrvt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxazyvlrk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdppifmxa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gjsejfrbl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gqkiqqjow.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gnsfagrlt.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/ghrvtotbf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghdfgizxt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ggjyqopae.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gnpmpvhol.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gbfudyxrw.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gokkwwpmf.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gnodfwdfg.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gndynxwus.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gafqgymqn.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gizbixkkk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gjrzcvpdj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gaqivyplx.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gxdmlbzmg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gfxvfksyd.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gkixxqxnv.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gmhotuqdl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/grqqgvmdn.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gphuqqppy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gnnlryhdy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbgolowri.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gthetezhl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmwdibmsy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpohlgcfc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gznivirqh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwqqrfyjs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glohfwcpj.sHtML


<!-- 参考信息 -->