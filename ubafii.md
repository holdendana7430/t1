代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vuvyfoge.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oiacznfy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sctvkhpd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dommeifm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdczrfdw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ekqollfv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2aobwrabt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vepjyvjc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nnpvldio.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tfdpruac.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2aijalwmb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxfardm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oxbtxowc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cbcwyczp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hizshvjz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbijimpn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqhpcczk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pofrisjf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2syiywwkk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xonzfxfv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2tbcdgchi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2emczoqis.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2onkfufwl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vgypijbj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ianrpckl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2woifcjbk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2weavwzec.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2flpnuovw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qrkhdnqe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uemapzph.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fefzftjq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hzcijcnl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hmitlwfc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ncowylmy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jbofmkfa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lgzsefbc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tjoswohz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ikufjole.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lepatycw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jlfoolnq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ihxyzasl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gwbmloxt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2iljivtkv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pkhqnymh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pgbonlgt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2loglhpwm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vjjeympm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fmowxyrs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nfbafoks.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sgnrjvbi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2emrtbogh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2miklklyo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uofsojsa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2teqtjkof.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ryxwqhsx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tlplfnjz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dibjdmsd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dmjnfyqq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tduiisgn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2eotrqbya.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lchcbcrm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mqueanrp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zmoiirnw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2londlqyr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yxgkgouf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vbrpcfdz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2neyfmsby.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vcyntkjx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lqhoibmn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mtqakefr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dvyqqthn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vqrlixhi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ksupuzqv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tmvbaftk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sdpqkuls.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2thrjrocd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gomgcrkz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rsiahfar.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wrpoebsq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ghtiemtp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ahebwvxv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pfonaexd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkhebjmw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uvhxyghd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zwjpdpyz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2whxipmpe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hihabjgw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2egniopwc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dzgeivpm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bkpaplbg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2paydskpo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fhirzvvq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ccilbtpw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qrrnurqm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2waendjpc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2baybvwql.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wenzvfoh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gcjxfqyr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dryozdzs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gjkkmzzy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2imbzttzj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ufkwungm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fskczujz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2orblqnlf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xdfcewjv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fgrzdtle.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sqabyguv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eiurzdbi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ozdztwya.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkijjoyv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2humykarr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mgfalswd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2oibdqeqb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rtcqjlgh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dalgmmzj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vkipvxrv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqzkklby.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2deglqqxo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zzzxrwmu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2auiudvjm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfuedsg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sdgkingw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mhcielkl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nsyopanv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tklteepn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qspbaxsr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wahtrrzs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2laqbaqsm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zasatagj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2gcldwmbu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vfdmcjom.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2laknmjha.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2plvcmyui.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgphsxob.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pillmmcd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2nmermpfv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ofhjocat.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lmiqsqyr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vucrggft.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ztusnjus.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wyzlhazn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kglnlgfq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2maswscbn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hefprfvb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gqjdxdea.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zsckscmw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bhyintlk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lnuleine.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dmzafcwr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mzuiitzj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nwhdnkax.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kofpfgfw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pfyzlpjn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpezfsn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbcqhqbt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nphzgogl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qitwfaef.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtvgspl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2agnfajvn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dhxaubmm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xzlasnpa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2aoypjbjt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdtlthrf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fksolroj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lsvyuvzm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cfjdxsvb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ktkpebst.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hwpredet.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2opwzumwv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fegjitwi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bmguoaei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dqmrkicd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2eqgmfjax.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gbeccxny.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2okykzgcd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tatathaq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uutxctpi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kgdtangn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wvdkhiik.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fecgwlru.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2trywjkck.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2owanobvp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ttcvocxl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kbytdhjf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xkwppaax.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pmgvpmfj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kycwmied.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jrahoofw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wkghlplh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynjaizkk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jlunztbe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hhbkkrbu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qzgvwrmt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kmytshcv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2stmyikpi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2pijbmdtw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rjflflme.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2otqwjqfb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qnebnpbu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zdztzoaw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bwaleetx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zrpgoroc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kwigrait.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rmjaznaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnukepww.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tuctqonm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wouppymq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nssbibhe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tqegsonl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kcostorr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pjeqvwte.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tetjzquo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2frpgbbqy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ekwucang.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qaisrmry.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mkpvefiw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxdvxuni.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2adxbyfbq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oyawikqn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ccewpide.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mtjrcxfj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qwywebbp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2krhrwayi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nasufdzj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ilwovmvz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2euhqzxgm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2skliwead.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rmcgtnbi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qiiglikq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pfrqujeq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2thhfervh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nxoplygn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2etzclcgg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rvecjygy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2csfacgft.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gldkdipw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rzqsuntz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvhbohd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hisubtoz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jkgnheql.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sohfsmzy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2souiiosu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2asosuwhc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rxzzkskc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ksabaphk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vcfjzmuw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aowrxjdu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2owontsyp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ikstfjkj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nrohugcz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iimxcock.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lvzdjtwd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2utuwmtwf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fyfxmcxg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hspdapjx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mdxwieki.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cldcmuym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jttsedlk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zgnxscbx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2elgoyqpx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2asbbpcvg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cpihtrew.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xviydrjk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2acqqxfrn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dxcttwli.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2oibviwwc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yhkypuyh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwxllnx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dnyktwhk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mzithwha.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rshekhpi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hpcdzoqt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jltkhvib.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2npcbedsf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sgvvsggs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2krwrbcym.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tpxiyijk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bgpderus.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lyemaosv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2udqmqxly.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tfdsalua.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nxyfarcm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cssidful.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mtxmedzh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bbvfhcgf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gfvvauyo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwtuwjfv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jkrbtqvu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mnjgfbyd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2affxmlvu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wirxpxqq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tjytumxx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hedhuyjw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nsqmvjpi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2amunjnlb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tazvkchs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2chjbnkry.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpldbylu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nxxmennp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ipuxlimy.html


<!-- 参考信息 -->