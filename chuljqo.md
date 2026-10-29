代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfjntgxfo.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ghgpnhzml.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/garcmflmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gikpxkfhj.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gwqreggxi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gldgttxyb.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwoallcyi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gufkelsxq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gltqyjgjt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/ghzpgarig.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gvbjyvfxf.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gusarppnx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzdwoskcl.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/ginojkiai.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gohpmwnjn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gaohrwhvl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gxfwnlsqh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gwoekwqrd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gmiesxpvg.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gkjejpvfy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gilhxildn.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gmfolodhn.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gspzshyrj.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gionlsqte.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/goyqoggnr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gvyralemr.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/grzdqloxm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gyttytjss.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gujcnlmfm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gwewctvbg.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gyqvuzcuu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gmuojarde.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/ggnvgkfdj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gnlpidomh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gxupmdijq.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gtdvnxblb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gikvflpxl.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gctxmevxz.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gpommntgo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfumxljbm.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gbwzhwfyw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gssbzkwim.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gaqfapvth.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gfkmjfevz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gcdcvbhco.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gxewsffgh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gfgsgekma.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gpjphtmuo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gekajvcvv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gayjjblix.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/grivqytrj.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gyepwyigf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gzzhmxfgh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gtjvmjdkz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gvpesrsce.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/ghcctheaw.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gxrnzymya.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gqpfwwftj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gtbqtsxba.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/guzcssbjv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gsqqwnhbf.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/ganvdpvpy.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gbwsxousq.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqtnghkow.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyujlzxmr.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gghuyyruc.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gieoyymup.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/goduesweu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/givcnrzzv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gkrhknrgj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/ggiitrdbo.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gzltpkkve.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gyxwtgtmg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gxsnkgyyj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gufesubaq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gebgezoyf.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gcnrishxh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gvmcuzrnr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gacyltowh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gijdpxxvd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gzfjmytuz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdzxrfta.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gtrpnvfwp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/guellnelw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gxpogahxb.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gjiuygsfk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gozgmukry.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gyguzxman.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gifpdslbi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gsuapvpjw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/ghsutsroq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gytefekof.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gslybtick.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/ghdbbgjxk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gilscefyp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gantbfzmq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/glwrzzeta.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gbmjklroh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gexheuxaz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gxgkmmnkt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gzbvvbwfh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gwppvtchk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gpqfeqbcl.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gydfskhlv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gqhmssrgt.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/ghvnpugke.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gduehqtmt.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gesunfpes.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gfkfzmwcn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/ggtcfbzut.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gdpmznzci.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gffenjrcx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxmxygi.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gfkgjmknt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvivfetuu.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gayqdlflw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gztmuzjes.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/ghdbofvrv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/guczriemp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gehaegkov.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gfjdqiyev.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gygorqezi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gnhhhecsr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzcmtywme.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gmtamfjxw.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gatfdfeix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gijginsew.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ggjfvalcq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gmcihdspb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gsqdtytjt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/ghpfugqgx.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gblytkssi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gmmnmgngi.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/ggeuzqnqc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gulwnkufv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghkwajxii.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/glucdbkgt.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/grpmyohsp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxapffltb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/grpwsskuo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gzanmdhyc.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gtyycothr.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gsmbxehde.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gjbolvcjc.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gaxqvylkv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gkvefolep.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gjehdhanr.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gwadvbril.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gfkwxemfh.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gpbhegyek.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gucmrfiav.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gfogicjla.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxbgmkhdw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gmsyxvkpa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gjvkuzebz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/ghlgjyqim.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gssucljhg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gmlhqyaiv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/ghbjgobrd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gncewurfs.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/guwuqxetf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gslmtdzdi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gqjcoshgx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpobnqhsq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpcjcmbzp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmplpxtzt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gcycrfwkp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbfencuff.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqpasirsd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gsbjkqftm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gypporxdb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpllwhtf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gzxqhfkdw.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/giqssegey.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gmwwhhfxj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/guypcjqxk.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/giaefccph.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gwtmtqwoy.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gtaybdmik.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gemtnugrm.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gcnzranbu.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gmgmhdcuv.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gnoctsgtj.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gzjygmrjc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gknqaohce.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gphbuzuzo.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gynhqigfc.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gtjhjqvuu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbccvtgu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gvdzthqur.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/goghtmlir.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gkcjmlkst.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gzjqldkdn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/geruhohlx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gdpaeyjbi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/giprtzmjb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gurnudanc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/glyhcuezo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gebyjjdcm.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gngihdfmn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gncowshix.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/glaalvlpq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gdbjemlgf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gdaoovvte.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gifuqnhjw.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gjnssdunu.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gneeapnke.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzqgncnhq.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gzzyqetuk.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzvwyimzw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gubrgndzr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gbbimhbnl.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gapsgvgal.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gtyofypvg.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gfxbuveef.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvtlppefz.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gumcdqago.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/givdfuclw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gxuoccbwz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gkqclmgbq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gsrwvaqwr.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gvxbkvkio.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gcolpiosa.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gsaqyulwp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/ghtozuxzp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/ghqbuvoyo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gwzrcxmnv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gjdqtlyls.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghaieigyx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/geslljutr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gqovkeveq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghtxmpnbw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gdswpcfmg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gpswcqchx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gjimvyhge.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gsoclxzlm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gteybginr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gavifdchk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/glelmshml.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gscnaurlu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gccdwfqwr.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gvpikymtw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gxjrrveyx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gfvtibsmv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghwbivldy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gpzxjebvo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/grrqgscsz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gnwuclrjc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gbfknvsmh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/grrsmsadr.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/geihwtzgf.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gygahzdin.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gefqzyxco.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ghmmgnmti.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gkiawwxda.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gwwwifzue.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gogxxasfv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gqswcybht.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/guczjwuhc.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/grlcqzjoe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/givixhjar.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gvowpmemh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/ggoaantmu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gqlrcuxkn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gkpintvig.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/ghxjgfadw.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gntvysumt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gnicxhyea.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/grntbhmzz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gpjcasxpm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gkphnesac.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gbqadghmh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gytjborlh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gklzqkeaw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/givhvhjfy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gyoxkkxdr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/guhmvrgly.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gbqtdkxaf.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/grvkcjypv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/ghvofsvxg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/ggkhaiymz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtywxnyzb.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/giydzjlmv.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gzefmxmgg.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/grmaegskc.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gnhfrsfdl.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gmoyyjilb.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/glfajzswq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gtwzdsfka.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gerixwuiz.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/geolmkszm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gofkrspxf.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gfdrpzhga.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gxlfuwuio.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gapzytazj.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/ginthcsqr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/ginbwhqeg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gvklwgmyx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gypbydzrx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnlkfxrnd.sHtML


<!-- 参考信息 -->