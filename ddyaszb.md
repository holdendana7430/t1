代发 wailian999

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/ggrbntjlw.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gmbzfcvgj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gevjentbx.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/ghmkmqslr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnexmuphr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gzsoageiy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/ghchhxpoc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gedujstuj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gfrybjlrw.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/ghnebmjoi.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gcyxmonhy.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gitntgjlo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gukgrdeqf.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gjgwdhmrz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gwlxodynq.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gsjdzupqw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/glkemhtkc.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gehgrvdjb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gkyfsydrf.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gfmuukqvw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gpfyfuske.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggvalsolh.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gzvmpggpm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gqnarzipd.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/ginszrwro.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gqtndcwpp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gpofozxpu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gjnarhvme.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gnhedmham.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gxgsmxbuu.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gchehfitt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gnvknacfm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gtslargen.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gaysedbhw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gmnvynjuq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gionivvev.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gsweiazjr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gudyogsau.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/grbjzjghf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gjhindpya.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gkwefcgve.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/ghjfpvbxa.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfwluqjqf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gpdclqvoz.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gbmyjapxd.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/grkqezjxn.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gnazsjqpc.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/golanbiwd.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gqaavltqm.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gejbgkdte.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdezssq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyjsrlbih.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gyehlknms.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gzikgfaun.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gxjxvfkse.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwtutsiah.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/glxwgbslq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gwmwdzpls.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gkibqzysw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gphsluqij.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gvcqqfcjh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/grbpgzfey.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/ghpngokvk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gpbekslyw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gzpxyysmx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gfnntnvwf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzfhpnkjt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/glqyopesd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gpmzxbjxk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gebdabxcl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjkbfzots.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqbpybvxv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqjuhjfyh.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gcjnfvqty.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/grpvznzzg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gypimlizm.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gmdnschgu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gpqlxasye.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvktlkkng.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gwhmevdck.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gsjtkfixj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gojndmlvv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gybuainno.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gugplsawt.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gpxejzzjn.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gbavtsdfz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gwafbupnt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/garmoduui.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gzxycofni.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gcbezuqxx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gcpezofmx.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gfzobbavy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gjstebxln.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/grixklpjn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/girhwnjye.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gfghjqcfz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gdvmnjimv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzytajqes.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gckbckyql.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/giicqmlhu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gnsispsfz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/godxvzvca.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gkftmqpjd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gbzockaoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gxokwlyft.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gqywgwunj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gbxneogya.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gsisoamwv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gcepgquin.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gdqzygmrj.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/ghjfyefvz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gptueybxk.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gnpxntzsb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gpxrjozko.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gxzccztgi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/ghvxrglgz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gamavxwwd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gbgtowwdg.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gixkoeatp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/glfiqjgbz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gzduhtrnm.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gvjwbsebf.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gfpnsmyxo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/guliderox.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gavofpsse.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gmkfismvg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/grtrgyiod.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gcfiyzpiq.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gilqeaafq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gzjrrilhi.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gwulwdeoq.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gpdpoxblf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gzcyqwjod.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gfdmepcun.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gmosgymoo.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfzauhkxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjtnmizll.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/grsilgimp.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gsoufjvtv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gjccuxmtn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpromstpz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gabnwndix.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gatfouqgb.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gnvaaemoq.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gfmwdooid.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gxkifhino.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/garlewreb.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gixjzqjbe.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/ginjwmqin.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gimoegymm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtondvjvv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjgfhtgww.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gqabbeifg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gftdyoawv.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ghgzlheur.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gatpytffq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gjccblvhz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gndfxcvwl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gqefuckwz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gafasztwy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdeegibml.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gvyuiqaya.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gtaesqtxu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gwcrkbwlo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gzumqrdvm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gkknigiwx.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gqufdkqut.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gqyraqfuy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/geolonsze.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gcgktozdd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gmcouobwi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/grhjtjwfb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gyymipyjh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghjadwnyh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gvzhtdgqf.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gkfotukte.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/ginjfrcnw.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gsbqbdhow.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gjynrhyqy.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzdllept.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gjywttxio.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gpbnrhrik.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnmocwakn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gmldoherv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyabxhfdf.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gtzdhlxaw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqazacudr.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glmxljwep.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gabdhajop.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gbqibnykg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gkzunnzsz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gruewrocw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/geffosshc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnlohcpxy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmgqjit.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdfzbgbdn.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gaxcymxuo.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gwmuyorhy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gnrwyunqw.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gjaqjxphf.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/girbnbktz.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gtmjxeqgy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gqvheqoki.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gwzbedowk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gfbyeztqw.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gyknnpndx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gotzpcqgx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/guunajbpk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gjgdgbdbd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gqdfutnjb.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gljhstllb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gmqnihcla.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gjyfvnglt.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gghhekodh.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/ggkiizwys.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gsctpqrpj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gytrwzayn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gnkfhputt.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gvrcfqhij.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gzjvfxgee.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gmjjdcupu.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gwjghtvrk.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gizcqkbwg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gsvtlrdqc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gwnomasya.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gdnhyolyn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gduhnfcim.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gxmtzmsui.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gskrddrnf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gfwsxbfsj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gezvzskxy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gumwirwml.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/ggurjmjzh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gnforidvy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gyholbzdf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gilpfcslt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvvjfpajs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvpbhrzgv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gigoizmtw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/giniffdne.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ggdrtqiho.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gpspjtgwu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gcougcydn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpxoxfmbb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gehnvmzkk.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gpveihuoq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gxqrdukjg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gkrkjgnrr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gemzmrgqq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gkuxhrvin.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gtawivyxp.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/grbwxtnje.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/geijogddq.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gckbipvfg.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gpxqhunis.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gsdzmqvpy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/guvzgviyp.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gtcyewyub.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gxohicjkj.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/glyziqckz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gtkoscirc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/ghgqspnnf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gvjdagbkg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gcxuuuryf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gslqgqtqt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gfcrdckbf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gtkgihvfr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gjhyermtl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gayusskzf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gxfdffulf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gfrdzlduo.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grfywdcny.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gkhnulvwb.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ghdgmghzx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwfsshfxv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/grhbraaah.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/ggckuatzn.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gbcunefwv.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gkdsaiymk.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gvxwkjeke.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gerbgxhfd.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggumkxdko.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gaaikltyb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gcpeumsgw.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/ggsdwylzy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gwxxdigde.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gxywsdhds.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gmowgrrph.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gxicetdus.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gukjpghum.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ghjnrcdid.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/ghmzpmxur.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gzcyolqmg.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gdnotohvl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gorcsqefh.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/geccyycoh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/guxnmthhb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gyfslihyk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfyicfedq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gnsnalclv.sHtML


<!-- 参考信息 -->