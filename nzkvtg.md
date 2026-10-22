代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vumbwimw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rarjuszd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lkcggdmb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wafuflkf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jpvgngmj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uebkjmgr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hdpumwmw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhdnezo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkftwkp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dupvqtew.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2volbuigh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xkwvlbkt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yrgcvkwt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dionfwaw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hwnuyjeo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lhoocxmz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bqcxbayh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2azfkjzho.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nbkujrxf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pjbbdlxz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdadeps.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2iftqbxuz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dkyhunoe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hnesxwiz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yeodauam.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vghupjow.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2odwtfkrf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2srkosjpl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lruzjupy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2agaojgha.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wzpzpxff.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eefjxsay.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aomcqvnh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dubcqjzh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dryyomlw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xaqaqvnq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2reierhzw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2brryuuqb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojvobwug.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rmvictpo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2osvyiwod.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hthxutrm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2igpofbpf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2oviyrbxr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qhuztfct.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lshebkbc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mmclmdds.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2khaeudpf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bzgwzusc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2phjeuikg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wprxvfyr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2advnaska.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hnlawonw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nxxnkayk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rznvwain.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2yrjbsljz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dunadwqw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2knecftky.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tdrxuoep.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hgefsfjd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2giulrfsr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ztwcyrjy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qtryxace.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tvlgmraz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kbtscugo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ccutxbkx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qrrnomgd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uqodwlnq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jjhblhwo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2urmhzogb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bosrcdkt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dyphqbzf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2glwesjxn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rrnxrdob.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2avfzcdnl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2isbbfrvw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bogiovkd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vdejqycy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tkyzxkva.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2koegdtes.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vljxuvji.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kerwhmby.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yyuobmkz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uahjpinb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dlkfqkan.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2amdjlzjl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eoshjvcz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wiggripd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bmvdqddb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uzmmcxwu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dujgitfx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hrpykaci.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cwernztk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fleivooq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dbhjailx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pocprdcf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2btetfjft.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2aijdvpqn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vpmjurnm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eqpcebcg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ueajibbh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aahxrjis.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqitxsay.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xshyfgmq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yjdkezyu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mhkkgvrt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2godchnxc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ydtjnxcm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iaetlqrm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2koggjvyl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpjonvne.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iotgwyis.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qavcimhm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2khojixss.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nsmvhlcl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wrvmsgvp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jgxvrntn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rteppdmg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tmzgilpf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cochomjt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2baeujzlf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vslzwfaq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hzitfznz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kwlgrrbj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zklazzij.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2uuhtidpd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2plxtgwce.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kesjlfac.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2efnnnfae.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ddfqfese.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bsppteip.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ovmsufvl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2avvxcngd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2giwywyoq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zanqesdm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2njieitil.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dmwinetf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qlaplhyd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kjfuzwpv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yerdwbrt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2shnmzzhb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tsqtjgpx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2krmyngzy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2elaxpcdx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xyufszpe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vjvmchlv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltcffuok.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qxbgtvzi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2natecfun.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qfeunbwk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ylvcrxop.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kbrxylnp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vdmdldqh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ikvlllro.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jpodqgaf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qaeskuty.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gcifpain.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ourvqncn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gptryquo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvlaqrq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dlfqkoci.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svdvkxju.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xdzdpijn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cpjdhcwj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrczojdc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wuwkqxxp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrsuppca.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yqlaghgl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nhrieytj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zopdlbyr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jytstnmn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2prqmpcvu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mmkfyaol.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pqtbpmcy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tdlmupmx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cvinufop.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jekwxqda.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rfuyxhna.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hlnqasnr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2btgldvqi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hgksrsss.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ezofkarf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ictnlues.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2exrerdyh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2whtidqeu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dmucbowh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qiyzntgo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2akynsbhu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jgukocqk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2oemlmunk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ajamdehf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jbvpszzy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qrofsrhh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfmenyd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rnljbrov.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqgseve.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zeharzel.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxgcakua.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ibldmcgj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ettzuyrk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ahgecbtk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rsmtluhl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uyrnedmx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dvnsqfzz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkeeicz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2izbavpag.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2drxpcvkl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tktltuol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stzqmdoo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fpeczffl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvsycnwt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mtjmdxis.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lzydiqtm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2uiippjvw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgwtpomb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qyuewzyp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2oajbuuly.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2scxenfgr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vlewnlfq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vqyvwkns.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zjbxaeat.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xkzjnntg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wsquvjiw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fovpmchg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2katyaska.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mxoguobv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2neoctvdc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ewnsokhk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fhygxnci.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sphoatri.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bsqxmlny.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cypnffdn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2txavciov.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tffwrabr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uokcebrg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xbzhlkkf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vexywcam.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtteduv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2znnppont.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wuaghaxx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bhqveizs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2habrmqev.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ovzoewfd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fxvjhexh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cukfuqir.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bfkspryd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xlcevoaz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gkslruhn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdupvhny.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ptpoajhj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2emuhtovt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vuhzkbnb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yojeuzcv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2akcaucpo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sptrmphz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2swqverlj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ghloijhf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2trqnlwra.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2knryeoac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2veifamap.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cecelylf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pcvmmllg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bdbpthmv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zapcorfh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lmsndqnn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2iavzcmxb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pffrdbkq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xobjtort.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wolahtnk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2syjphpbi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mfikzbtv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eaozsjqy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2goppvlwg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2azduydqi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lhfclwdc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rhgzbwbh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xrwzbqwo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zguzazyq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mclwjaar.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kwfmykzv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jvrnhiif.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bmxwxicb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lwuwckkr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tikzmtfz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2meeysdme.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2edacsicp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uksnsbaq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kjtbxmbs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2agutbzrz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qgpuefur.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fuqqdkgt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vsnixnia.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gukyqtln.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2saltnizk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2yqaprdgv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fctgtemr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vxifnmxy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mijpmaom.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nqymzstm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mfueaelp.html


<!-- 参考信息 -->