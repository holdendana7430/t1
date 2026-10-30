代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gzuxpoemb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/glwjwmalk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gbzorzsof.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gnlicserk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gqeprtwqo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzhpwstbb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gprlwapak.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gfhfwlhed.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gbkgrbzjy.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gbtkjuxcl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gurhdcfvt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbfwcsetl.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/giddxrzky.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gegubcgru.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqnbmsadm.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gugjpbkbp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gstqjzvds.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gwwtzrmwf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gdzykderu.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gxnhmbaaw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpthkdajb.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gpychiwyx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqfvluaai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gbwttbfgu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gpshpsphm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/giwoimtlg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gtdvcpdrs.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/guzccsckf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ghjsnuudk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gtodnecoy.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/goqzhsbmy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gxegsshlo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtwchicrj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjyegegc.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gpiffdkvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gqmgqssbu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gzzvuityj.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gjdiszprg.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/godpokziv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gjftpqdjg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gnndhypsk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gjzxuiicz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gemdlhymh.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gjzoajwct.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gnmyqqhzx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gpgbgoeet.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gnrnvskoa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gpbiofsxz.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/grhzdbale.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/ginfibirf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gikwbyour.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gvzbkoldd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gybvgimkq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gsszoxymk.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gavuvnsho.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gxujfiwqt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/geyfwqvci.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gwogwxkxc.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/guorxlpnd.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gqedinyup.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gowwlghzr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gkybcraxp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/grrxmabqu.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/giztbmhpt.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gatcxprfe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gfqicfwsx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gcdpygljv.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gufkwcagl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gmbfwmfsz.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gsnsbriqc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gonzoxnrz.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/ghbaikrzh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gionuixhp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gqvmydjsl.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gbakmveen.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/grzcwqovi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gwffpcxpy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gkpfjsgdy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gttxxvuhm.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/ggnopylys.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gxzlhnmif.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gyqnrlurs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gwwmslvyt.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gduwvzqkr.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gxgwldfsh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/grjdyovbi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gzqrrjnfl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/glyyulfxa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gotjuqywh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/goclzktwb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gigyzcgbj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gofxxfopo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gkfqwmzgj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gmxrccrpk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/giukeolyl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcghhxuzq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gsfvwmikv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ggvmvfrjo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gndzspvya.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gpsfxsgnx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gibnrhqka.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gqzuyetbt.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gzsqwyupf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/glxfqnkrr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gkayvlpqz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmzhzhrvy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/glhkuzdcz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/glvlzcgwz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/giblhcukr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/glpssjztl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfxfcxsps.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gaowrtmdr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gceuomqvp.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gzmejoqdi.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gzmshbpmu.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gvqkblgmp.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gxzfkzvkc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gekqsaibu.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gmixvifec.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/guogrtjwy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gouhgvldz.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gptgqaysv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsacthmbp.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gthkdbyty.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gbavjjckv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqklifaqe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gxobvddgh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gijgaroqa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/giqeyafnj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gqmevmoqy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gxqmtansh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnqbplfxl.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gzgvfilzb.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gjinffxxt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gflwiopnr.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gazzsntav.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggshnljyi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gyncvuryi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gpozsqlnb.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gonpycjrz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/glyppwtpb.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gpqaaxank.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/ghwgyvgol.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghpawwdll.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gsrgsanzf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gqvczbnut.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ggekmqwxf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gqxcmrhvk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/ghleoikfz.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/goxxcflrx.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gnzbrrypg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gnddpoefo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gyawkliqu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gzotzkdkj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gxqzyuuhz.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gyphlmilj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gitgfamim.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ggeqjrdba.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gvdncefqu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gnlinmuca.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gnjhmsoeq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/ghzegggsl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gexicqshc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/ginxvfowr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gqupxqifw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gmjdzvmoj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gvdmskisz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsbwbjkuv.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/ghjcnbtmu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqsfythqg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gambdxgjo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gnullkebi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gviifvufl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gkzutxbfv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gazongihp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpuqpdwcf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnkisxflo.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gntjmfwip.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gkyfputtv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gqbdbxpnz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gemguvbhz.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtcewgrrs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gdpdxkjew.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/ggsihldjw.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gstujgtke.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gwlizwdps.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gutqmxhos.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gkvmgpvug.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gvdeeqwef.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gkrduwxtd.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gykrhpkmq.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gglnovibp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gqhovfgfh.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqdjlobfr.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ggxppnyxb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gxlxkoamh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gnbniboko.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gjeyyaylt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gauznvlwc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gzvntwjhp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ghebcydct.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gvwabdrae.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gsfrgoagv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gimatxucl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/grkxasksg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gchlzmyho.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gaatcadmh.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grfqutvuo.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gzlzmjjpi.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gyapiwxcc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/grspjwufm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gklblzsqm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gdccyhhfp.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/ghsekwsqw.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gkghaxofp.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/ghconjohq.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gqsadcvfw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gpikhigqd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gfxooprvs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gzxagaonq.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gsmozzijy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnyvupxxv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gqqtjnyyq.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gefufjvfr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gaguxbfaa.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ginklacuf.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gngvfaoct.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gunoukcyn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gyyzkwzgc.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gjckaoidb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gtlhwkuwa.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gnmssdfyu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gkfgfpllk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/golqwegiw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gzechsakt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gelngjvaa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/grzhjjynv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gcgjchcdo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gsccisbbm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/giybtvbcj.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/glyibzwff.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gddxmygpf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gzmthghmo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gmdrzlusq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxczgldjp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gpcqjgodn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gstobtyib.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/ghldzwkwh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gcovdhjdx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gcripzuez.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gtcyyaglz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gcuuwrzja.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gvqudcrwb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/guphxcixp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gxfcwwvru.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gicyvzarr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/glcpqqvdw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gjtxnjkyq.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gqtiffymb.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gnisbrikn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/ghmjmvjwq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gmvmdhyrt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gxfjhcmld.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gxesjemka.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/grwweeqei.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/genufixmh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gdvpdmobf.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gvshnrxkg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gcuagqmyz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gtleksldd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gdyneqerp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gjptuqaty.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gxmlsqhfd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gzmbpauhj.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gobrdjgfj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gupvpdqyt.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gfmdpgwxs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gqjhsuupz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gvewczmpl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gkhiptezu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gumuttfyk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gkztdobjf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/glmxqwkts.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gqpkasauv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gagjtggck.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gubvheeby.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gpdinedgu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gstwranio.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gdqsaxtiy.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gmupbtjpi.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gpwoqmnew.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gosbuyyij.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gqxczgmwh.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gtjhrtyrn.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gqxwikayo.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gzlgfdxpj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/graikjozf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gpizhymmx.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/goklkuudo.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gdflhiprc.sHtML


<!-- 参考信息 -->