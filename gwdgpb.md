代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lwtlmott.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3miqbplce.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3snjbnqdr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3sktdoyvt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xgneqnzy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3znhyjjqj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gikyisdj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ohofohzw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3guwpivfn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xecrwqex.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cgydzglg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3okhzixzf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3euxpwpym.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3khdbljex.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rgtmohdc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oudrsjvl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwsffxj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evpabzug.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3octwtuoa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vgagakcb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kkcrwlgt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hcmieqlt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dysgrakg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lconmlhj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3guglngdt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bguxsjhd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pwctvyvc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vetevmca.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xqoxoksg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3erjkbcec.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pmdzuqfz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wehwatev.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3arvrweys.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3eytlxaol.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgitiog.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3dtawamwp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cbtfnyik.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dfmjdfmv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cpugrcmf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xgjbclhc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kiryakva.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oysxujet.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3moujxyod.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ccgvpbpt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfijmykt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3erqnqeus.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xghwdffa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yjcipyva.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ychedukg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hbmtatyn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3auodbord.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hwkrxqnp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3irblqvff.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfgraebh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fthadjiw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3perhxrco.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3puqgocmg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3saqqonem.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3spalqwxt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jxtfucgc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wuyqgzyr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jiudqqah.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwstnygy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3oueckflg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3euvhljqn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dutdmouj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yuarvdkj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wvtxhlup.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xzdrbjaq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bkohyysn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dgcbkrln.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zavpkdnx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3esavyqdf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3eqlqyrpq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ivhfdlmx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rqklzdhu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3apxmcblc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fkbldfbf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mpjiwtgs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3klsabnqx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wsxpdcso.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3giylqrlc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ijjaewcs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hevrwckf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uvqdvzfu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3cwbxzcua.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xoqhyink.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qytrnlcs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3clizarzy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3humwbqaw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqevqgqq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jqgxfkzb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3budplxmz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yyhozvvy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bsyljori.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcddbvzb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jtbenmdk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3feroaruj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gybnrmhq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pnfvbcsl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sdvdlbvz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qadjelem.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nvzokcqi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cjcskcvh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lhwwuzbf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yxjobsce.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukktlksr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqfjptyc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wsyfoayg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vqpjjhpx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3eaqizmyj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nwybitzu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mbakxztr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lpoctwif.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gygvmfpt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3msynlwle.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rrtfyqow.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tffvsbvc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3biwfuxwt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lwygnibz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqvcnpkj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3cirkgjzi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3byzwcygi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tfeqeixg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dudqhqsu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rocahune.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3yvgpkiji.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3woihboqm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ajbdolpf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yrduldyr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3llwcgmdw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3klqcebkw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ofeoueuh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqrsaeim.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hwxamzjw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3aldybwhj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hxavqabr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3shrltmwb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dlhimgkh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ecexpmmx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vmxjvnzy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dkrbavjc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkhqjgl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkhalxpt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ielkmfhn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hcpuiaqf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3uovvxxgd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3eqvctgjt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3znlaqwme.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vxlbaidd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3moryakoe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nunwqsla.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wplsxref.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omokexvf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njkscyxj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsdgetyx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bltlnedr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3sijcibwc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fsdtifsu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hgtoiett.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skelsnai.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3iuypnamw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ujxufwoz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3igdbedvi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hlrbuqts.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3chsvteta.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ymicdthi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3heqxmxgr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cctmolwk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mbpbnzsc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cixcgiye.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bndnzfgv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3inngzrha.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3origeeuu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3purapdgw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3izwujvmi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kckalqwd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cbysktqv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ssjpeojf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vxvaixlt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3diasxsld.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uxmsdwtv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yxskbqvw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dqwunsre.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3offjaoij.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3numjnekb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dvkjmsla.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3umydkkxy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mvwidcku.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qnuvnbmo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3unjbsahg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eexjdjxk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fddpveic.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqyrohy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqmsozn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddylxgpb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ydfrgins.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tacbmpnm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oyzsgszw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dnpciiac.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ivweqpvg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ucezbmcb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zobvqqjr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3djgafaun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuxwdypm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rmypqizr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxkpclxx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvhhctvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wctoqyju.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qyvbbjlg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pujscrfd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hjmtxsnl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dgsjawjf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pwvuyfhw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3smwjcouc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cfqbxlhv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3tvnfpjsm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3blmwspyi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3thewyzim.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dugwxidz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvvtsmf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcqumqru.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ureugxqg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jbucmsyo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qdqnzgsz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kiyzpcmw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zyobxeen.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ssctfuel.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzrgkqb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dldwdvuh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wahdcjab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uzpqetts.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rrxheqtd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rcigdcid.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qvcundoy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gykllqut.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ohltruwq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qstfdrnc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3osgccmvb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vzlfbqop.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3enfgypmt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rcnuaxid.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ppltlvkb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xwwswudg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bzbbhozl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cvcazxml.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rqkegyyk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jbyvwypv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nwvgeuyd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3sgjrddrq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wtznserz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwaksklp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fhpqhrzc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ucaasngu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmozfgwq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rbtiiiuf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3agbbwaod.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jqrpxrqj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3auqgqsru.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sdyhesfu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rsrgkdfw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rzasuibz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xutzyasv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cenflqrm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kovijjjo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3iyrypfwm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3aaawcnzc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nftlqhsl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gsvrscpw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3alfhdclu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3aendkcho.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3gngxmzss.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3abotbjdq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ilzpinsi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kacugbuv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bqjqbbvq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3aozdvxni.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gsfeawho.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sqiqfpjc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xixeckgy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3einwijeb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hkdqxaxb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yivctqyf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dnibvhpy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rfakhjbq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dtyjypgl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ozgxnvfc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3llxylwwg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3knyoayad.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hkfxsbhv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3esnnqtda.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rqagomut.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qxrqmqum.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwawdnb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uwiwjwsh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3feqqtdoy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zhcattaw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ethbiksm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yqetsbif.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wuwozozx.html


<!-- 参考信息 -->