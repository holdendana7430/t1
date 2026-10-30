代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gmlgkurwa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gyppdjrll.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gqpzpdxtf.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gdknccxky.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnaplcrlt.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gpdiyhzli.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gdfaxcnws.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gxvzcthec.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/grnrpdjsp.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwiejxkvy.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gwxvdewsu.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gzucdamts.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gxzftsiow.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gwebfmtyv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gkttruzdd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvflxdhxz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gpbiqxjrp.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gfcvmzfpp.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gxamcwvno.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gebyqjugw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gvntvmosq.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gmpcmeedk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gtsyisbat.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gvrotpwfd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gheleakyj.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/goxyrddvv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gotnoxlvs.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gaketieud.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gpeodvbhd.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gbivzoidn.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gkgwqysap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ggdtwuaul.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gxcrpfbns.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gcoetuuax.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfwzhoy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gqjriwafe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcgcpfsag.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/grzutsxfb.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gipefcoro.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/goofxrkbl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/ghagnmlub.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gchzjspvs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gdingiqks.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gokfquioo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/guioxbkgb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gcehtquov.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gfsosoeku.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gefpjbrju.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gnlbsgwyk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gejcfuklr.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/geievhbjm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gsjfxsfso.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gphndbgoc.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gltazoujo.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gqteilqli.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghqplivxi.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gvglvuokf.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gjctaeddl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gnaozhrko.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gdvbexjlq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gpmermfoz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gojianqaq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/glyhjnxfy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaghmjgfn.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gidbgsjbs.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gjticelgp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gxqmnnxqx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gqbptwbnf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gwnbusmrz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gevdhbnmi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gyfhjqkhv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gqufoexfm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/genkpitrr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gqfmyzdtb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gtuzwjhyd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/grmeylapj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/ggylocvhx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gbcufvoxu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gtphtbccc.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gikmzpgsx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gwpaesiub.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gonqpcjqy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gybsajuwt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnbhndsgs.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gpuolnita.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gepgmzsmi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gdggncfpj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gsxrzdlgp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gyjnhbgaq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gaynfwrlm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gwpimuyif.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gwjbxybqb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gqtcftryo.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gvwdcsfrs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcygjcwpu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gvpfaraau.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/grtxgythd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gudjyzcna.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gqatvfgof.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gdroavijk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gvtsrkkqx.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gtytmnkeh.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gzarzezol.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsehlkjpe.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gsvaokfzo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gxnjbyohi.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gbkhgqhle.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gbvwjziey.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gmpdijinu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gfjdqzvhi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gptkkfxzx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gdstfahxx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gfhdsuoxb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gwvzztzjh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/goglfsnum.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/ggnotjczp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gmldyjoke.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gnsmvnjlv.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/grubwpivq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gykjbkqxz.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/glrugioto.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gfujipkil.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gknuzjjqb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gwwvusbot.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gugjdlboz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gjzykgnxh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gdrmzrebj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gggtdmiyc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gysyimhsw.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gbtswyife.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gmrmnuftz.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxjltfdge.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gmogudidq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gmhxevcxg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/ggmowxiaw.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gifttxscx.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gakeraryj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gmqruphrx.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gclpugtkh.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gogtxwhfw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/grhcxldkk.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gqcizdkje.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnbchuswk.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gdqoqzrlk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnvvvqfba.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gnvbtgbyy.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gbmnvfygw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gohthydnn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/grujdmopx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gnoqnpjze.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhlzknwh.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gbmlhhain.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gruzndonp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gshbsvtpa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gauovhupp.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gtedowuuc.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gbhqcrqyv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gywabcnve.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gprxqhzdj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gepfdhpjy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gevrzjqio.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gcolupxct.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gmmchlmlr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gdbkswhko.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gxiulmqnw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gedtlbtcy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gsaxmplyp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gvotuygcc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gfhaelmyg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmczakhlp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/giyawwtjg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gqjeacfys.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/grskzseqj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gonhlrfvh.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/goatjyvgd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gbjyhambe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/geloujbdn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gotpcvsfs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/goffxukaq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gzkfpmnat.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gfrpufput.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gkeiakhus.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gaenzlske.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gnatjwsmu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gfpfxhuce.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gvvszpstu.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gkcembtjf.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gsejxnnjf.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gixaoxosa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gfblvdaik.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gachubort.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gmgaljdcd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghmjqykes.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gtfprxwyq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkqsvfpfg.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gwodzteho.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gbjdofjlq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gwklewfov.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqpzuaprk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gfcutukfw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gumtsculz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gyesnuuae.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gelephryz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/glyigvxwj.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gasxidgpi.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gwdggejeh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gajmhbpgn.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gdpgrtlfu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gmepzlyzi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gdoaccque.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gcugeclyj.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/ghllbszas.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gqtfgdpag.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gpospwank.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gxpqokdgx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gqylwphpf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/guttkvvev.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gsqqvpqkh.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gtrpesboj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gwhimtgna.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gbereohke.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gfwndkffm.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gudrcmuwg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gasivcrrp.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gkyxktlqf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/guvjsugca.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gwsxjzcgm.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gtbtazwxt.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gmclqesso.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gxpxgkspx.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gjmekycgl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gbbcujfja.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gjqhqllsy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gzkaplmxl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gfrfviyry.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gltrsfqkk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/guvrnygjb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/ghtxsdwdp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gvwvuusqb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/giuoomtjn.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gwblgtway.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gicxzuldg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkjecseqs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzxjsebbb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqqvwogtg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gdjojlqsp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gzzasocja.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbbnyewnu.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggigedegn.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/grgihzvbr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gkpfyvvfp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gncohhazw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gqdqliioa.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gzdcfsaqw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gllzdtdfm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gvesbepge.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gdzretsrj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gwbjmhfwb.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gdulggzvc.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gfpacnfrq.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gpjuigcue.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gfwnpzhfd.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmelerucq.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gxzcwmhet.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gjvcipgfy.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/guhhmlgmd.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gjjxbtnjd.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gmzmegeot.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/ghmylotvq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gpridlisj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/girqxxcnc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gvbmkefox.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ghtvhbnvt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkfonhby.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnbnaofrz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gvnzrtnxp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gkienautj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grzbgmkyw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gzfzpfmcb.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gcvzoloul.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gubzaoehe.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/genvynsnl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gmssqghkw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlcszugr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gkwvehlsl.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gblzncvxw.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gzyowbsor.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gfntxduhk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwvkzidjo.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpvfpugdj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gothtyryg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gkbjszwsf.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gzgttdwnz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gjsoxcxet.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gjyvyuxwe.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfadthazr.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gbbucmdzj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gryjjyfyt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gmfarvmeq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gwfruehes.sHtML


<!-- 参考信息 -->