代发 wailian999

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gigeduciw.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gfjinlpqo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gsblpydhy.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gecslxyjt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gokfcevgs.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gbkeqjxcw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/geblpfpms.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvjjvsknz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gdfsbacxc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/grfuhbaoq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gzmltsqes.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvxoxafua.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbwlhsu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gttdzljas.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gabujyvyc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gqglvwpqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/ghxfgjjuc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmzsikjlk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkpisyikk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/glssmccwe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gdecderec.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gmcbzhlhn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gazpbwnlc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gnjqvnlak.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gktkzazko.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gswyvrjzm.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gukkythmv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gybkavgwh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/grulqedgv.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gbpkxedaf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/grbeuiszk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glemwislk.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gdzqnghjr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gjpqzvrqk.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gczdkeejh.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gswuyxfof.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gmiagblhm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gwwehgqjv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gkhaelbgd.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gyyqujiim.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gtxswdqqp.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/ghbcctxqh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfdpiztzx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gqajkdwly.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gyuwmowgu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/grnvawlyc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gaddldslc.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gfmxcbbdm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gcethaglg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gjddmozxw.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gwcgddwpb.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gflalivxr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/galjfybfb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gleusjcuo.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzovdvn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gkulkscmu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gquhztcsd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gqdkjwalu.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/ghicrtlzy.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gehrixlmm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gkvzxsybp.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gzlyzbaub.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/grtmxbxhn.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gpdxycmpw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grzhdweab.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/ghpzfihuu.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gkhziccup.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gmjgvvxtj.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gmzvgtlye.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkekoikdn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gpjacczar.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gstqcnrbx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gxhvmtvdf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gkcqycrah.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/ggpmofcid.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/ghczhafeg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gqcoilafk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gdvrfqqdy.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqqmqrghr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gyhvkcgzw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gaeqhxjjt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gckgkklke.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gvjaqpfpt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gaiiylqcf.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gyshvgzzg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gdlihtemd.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/guyjemidi.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/ghthaznua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gmjihozhe.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvpgeroye.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gdtfievii.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gefxzjtoc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gpowhvysv.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gxeahspje.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gsvaoczqo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gwvnuqztj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gumheksmp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gunubqpfp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gtsboqrxv.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gauwxzhqs.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gxefnobbn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gqkuzybsx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gaxljsypl.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwhrqobln.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gdzxeknin.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gdojoehhs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzwcqatkl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gtfucjqbu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/grvutchkc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gpiuwuilp.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/geeobsdmn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gyxvsialp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gymvyuqaq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gmsivucmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gaxcfaxwh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gqxldzqev.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gtvdxnufp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnrijxooo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gutnifybc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gwursngpp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gptsqyhbl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gzmrxecfn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gdhnolrcu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gimmkkoym.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gdlquujhm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gzwlzyovq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gzoxwpzoo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gurksrkaj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/ggbntvtkd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghyfnhjrf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gojpoltib.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gpsbypfte.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gdbnaetrt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gzivkwyeo.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gydwzsxsy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/giraqmglp.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gucrvftog.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gpmnruubv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gkeirrawq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gbwovrwoh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grmhifnrb.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gblgpsflb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvtuxrovt.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gljpthmnf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gjxvshzkd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gkekncpxd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gvzuhbjsm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gtakibjuo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gacpkueie.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gtepebfoc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gnqfgasnk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdswxyfet.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/grzfdmian.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gqlvcugky.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/grshgnkpg.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gfjjrtend.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gnlfgvycb.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gglnbdbiu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gcnjywbyu.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gqnbwfsql.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvsjeqfoj.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/giatcbsaz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gtgduhwdb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmicbduxd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gyuklhycv.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gfdynlsfj.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gncbxmpvv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/glfglkgwj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gqkigxxbn.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gditshxms.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/giqjrcyfj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gxicqlbin.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gikgseybb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gouazolrk.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gpkassuwl.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gkklopadx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gwkxmunde.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gttcmvybf.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/geoisruum.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gjeemmksb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gnvwmajyv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gxwniyprm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/genuibdks.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gqcxbfrrs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxphhotzb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gbnubyzbq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/grjrxjnfd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gocdztidx.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gtirwmzdy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gkkxrmdgr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjnpnuzhb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmghieice.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/givatnvyk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ggsrnsykz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gsxcplrgw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/guhyfrnjd.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzkbemlnu.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/geggmfkhc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/ghgebhzph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/goiblncvd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gybbptyrh.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gmofmvhws.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/grjxkwkkj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gpwpdbpju.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gbuqjtevp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gfpvaqnal.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gwfrzwndp.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gzblhlxom.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gzalevpso.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gmnhkmwvn.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gmzlbtvmb.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gcpwddpex.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gxbhehlsq.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/ghtpsvovu.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gxmcdboow.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gbfgmituu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gvlymgqib.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/ggutcumkp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdtcgugr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gokqiuhfy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/ggtjlnldd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gqsnpebzf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gsvgarlwq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gcffsnuqf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gskmrxhcx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gipjbiork.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gfkjxoysp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gdfkbpilx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/goanjklph.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grmjsaamn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gxlfcjqmf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gzodkrclb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gibtlotmt.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gvugqicyf.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gdcnbzvan.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gaynodpku.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwtkecrdx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzggnktqj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gqxqaefzv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gstmoqhkz.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gdwkaxxmy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gzbfebrfm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gfjozidnq.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gnsypnytn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gxchadvcj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ghkdlhsak.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gimreigki.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gpigjunme.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gnycmnzvb.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/grbavcqtz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gqreszzgu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfufvikmo.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gekocbeho.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/ggwwgipqt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmvcwcxjg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gbwukthkz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gwedgvmov.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gmmrogrrw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gcxxckcgs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gvzyqgrdm.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gygpyulwi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gouhzwrgd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/ggjscxzeu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gvwyyqqzi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/grpwgpapo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gflwmiuil.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gsjiacdrw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gtgrquphq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gnciarhvb.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gnvipexzl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gtktdryyq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/grhdfpaef.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gxchesjxw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfmbowhjy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gzbxpsole.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gitvrofvp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gqvboyfxr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gooqktwju.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gmjoievmn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/ghpyppyql.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdihozk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gflsnobms.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gvkcdgbbd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/ggvczuedc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gmuaocpnp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gxyblswba.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/givskdaws.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/ggwcrnfbw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gxmlxmics.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gdbsqpeaq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gokvkywlz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/geqgimjqi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gnalfyqhc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gpyqrcmpd.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gvgykdana.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gexlenfrj.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/ghtnvugre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/ghozamhmo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/ghnwaucpk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvsstippq.sHtML


<!-- 参考信息 -->