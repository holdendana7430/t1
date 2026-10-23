代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3itwxymun.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nhjukvpp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3elmooqzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3faxwlcfa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jnqkkkry.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nrjzthfj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vbxeejfs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3oyungqud.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dhzxmcne.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fysrikxx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hfaniulr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fcobeiba.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kzqglxrz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hvbkrxlc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lwypjmfr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eahjufug.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3siibrceb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehrvmwza.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zuybxgln.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jmgyrtqt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3odhzxwxt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxxvajbt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3itxjvlyb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pxhyjsrv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ousudjcb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3kenhywia.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vocywadt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qgmhgwcm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lmuupelr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jxigveks.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3oifyeypi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mmrqorni.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhwddwqq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3houijfkj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3coaetybz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwnowfw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nihpkvax.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rwphxjmp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecwpgvoi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yusjgvzg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zokehyqe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ybpkfbkq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bsrpiuvb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zseypuuu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htjjovub.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rcoehcmr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tpvgpoab.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kmbqxmtq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwssziox.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jujqqneu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zxsziuuw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kgpkysne.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3brgnlgrn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ezwlmvvs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kzwbgkcn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wzptdjxn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zhcrmpvp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rpbrhxri.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tibtlgab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qzkckwaq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tovhpsso.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wuofosfj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yfkiuuti.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jsffzucx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mxwzoheq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zgkxhijr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3uamqctjo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hkymqlqc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fngigzkd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kktkemyc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uozbtlrm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pntwxixv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tjorwrmu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cvrwkesk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hoaphlvx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3omfuzdzf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brordnyo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qsbbbojw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ioyewlnf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oiqvtkhk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tvtzlovz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cxelvoro.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfcvrvr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nflsbrah.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3osrbglyg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3exlxkbzs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mxevgonw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gbpsopih.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gimiebeu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkbhaanl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfkzhpc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfotdnmj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3esxtjctv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftdjhmvk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mosmtaig.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yuulgjet.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jhblukrd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fufwofhl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3iefrnuxu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wykirdhz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xtxblgrc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jynchqqf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fvarwmzr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3sqasxepy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3obikwlym.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zrrwcnqk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3knmdknqq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hotpxyco.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3feaerhcj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bejpwpva.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ytsktass.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hhliytrz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kdohxbef.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ijagjxrk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dqlydweq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epwlddzy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qubtmfff.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbbxtwmj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mfzyzfpn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3szyhqtqz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmqykgmr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xbtktxru.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bzudrkug.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xugzzhei.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3csqwtbzm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3muvapxaw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pwfhgteb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ncqvfmdk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gciobwnr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3nygdcqdu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3cmoajlay.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lwhhdfsl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ukznqoqz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qmdlacch.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3btljsqqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ndrfwvtx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qtstuinj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3cyazjjqh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3eecneare.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nfxsxxpj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3umragwvg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dcmeynmr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cvwratfy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3sagjomnx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dovriwyd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hbdftpov.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cjqzpyju.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jhpebmlk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3alzngkor.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3skkdgkoo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mzieocau.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mwwwpogu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ozxsmfpp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ubsatmev.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yiebnbym.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuceogpb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lvwmjzss.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdrqwenc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ymofqnso.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jmssizzu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oeijjzxg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qqvtdqyn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xyykcwhp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3icmbutsm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3blauyssf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gxeoyqvs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rstnyhww.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jcggeghg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lqtjqqbd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3odoiknfc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3popmewme.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uwyimycz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eeicidcs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3snanzgpr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cpvzuwws.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ihncxreb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nqxuojpa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wrogaiuf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iulczncb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bxygjvdk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwfzsxv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3udrvwiaw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fjaaudcq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hpsrmvzf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3brbinexo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gafxdgwi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jeteifpa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3aqfeqnux.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wyoxjmgc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aepkixcp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nsitqwmy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsqvbneu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rhwqhydn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkxtnwe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3arjgidxp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pdxsthlx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zqhsibap.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qpipyqkc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nfcresvy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fgpyjsmz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kjbvwrid.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vxbgdgvh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dzdtmmkm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bzbggril.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpxwwenn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tkjtgwpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyqvdikg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emtjnxlq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hpqdcrhj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pmlpwolc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tnazyydh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3oqioyhbn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vyyklxua.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qnwvxsoc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3npjwwaoy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ykecmmau.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvhxfogo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ldfvezyx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qrclzcxz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uysmkszn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrrjnsgo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzlcxjri.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3idahmyxz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mlvgmmvj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ccklpjvh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3egeuxfnz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rlesjrma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bqeirrfo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lsjtdtqk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3adzmrdmy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbbkcwa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uecuwogl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3axtgftvv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ildrxoel.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dwiqtcgs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ydhvfzvf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ngsmpujs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tszxottw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gszcpomm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nzosnlmp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mmxnoggz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3slefhezx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3obeduivx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ialtphtn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mrbvcvre.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xxskinnv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nptkvedg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qsdzwuul.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yuffmsdr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3znvjsmjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3myfeaotb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pwbkwido.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mzanqbap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bdnsjcxg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3axlsycoh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bwjxgepm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hisrquoi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xmdzevjb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kyntkpmc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zkvydgrw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bjwabeni.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xavvglrg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tfpteppb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eslndzuz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wifbrevc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3epjphvxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vjnyjbyr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smxnifru.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3thbrsytq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jldubwbs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tzyoxxfm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqwaudz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sjxtnshj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pxgvvzrs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ywbcokfi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nudxulek.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xrbulunn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cdpbjfpu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bdtdkbht.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3nmlqzimz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ojjggjdf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3djxnxrnk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ihkiweug.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kbvskmkc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vfjhxhvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rsudlylj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3aiwvdcqy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hupntfmp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bfzrglgo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ndaprykv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3denzsrxi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3acwdnkfr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iedojths.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3btvatzop.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3govltijv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xsdlpnqw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dnqtbwtc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yhkgimjc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mbpekvsx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dqufokrm.html


<!-- 参考信息 -->