代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nehnvmnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ororupqi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gxkebsqw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mqrepmhi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gjajlnki.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fkrnbdnc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xxuzcaqo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bijtvdhq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3omgoxyqi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eieinlrw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3txtpxlcc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hipqqjct.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ysqdddiq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pnoroseb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nkyleyos.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrrqersk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gnddpvaj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lesimlhw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lpheghop.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3iorifsdp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rbgebxea.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yyptxwfy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3roatjkom.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fiwqmzwd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yumcmzeq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3owofkslu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzwqygx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vxtxfkbk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ungxikma.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tqxnonsa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bndwamqp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3graewvjl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3inohdiew.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qeitlvcb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pvpsayse.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mrhgtixs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lywuidtt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3snqfzhir.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zrfqswqb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sxhicjip.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3etxlxjgd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3beiejgil.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3prwabsyf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cwlbvodb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3efdhrdhh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ihbohuuf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3szbdpeyc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgqanqas.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewrasapa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3usfzomik.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3svsuyrri.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3omcywppz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3endlwhiq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sbfzriwx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xlxxrxqu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wsouusvd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mwpgficq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3evbhxnot.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xqidplfk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hktqqpsv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3txtqnbzo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iouvhiup.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3blmbkdmu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uqflvoff.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qopwjjdt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3elvpengd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3evwjdrdj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rigjvfup.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hpuiowie.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wzimeddl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmzlnjvm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uczjsqgb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kkziqxvq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ytneozkg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hirfgtcv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rijncyuk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ajqeuobm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gqrhgwzu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3fnlxcjbf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3byvcrhiy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjihwqa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yezzpahm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zhiekhng.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mmulcixj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3quzltiyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxfczrvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtdbqob.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fqocntew.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jvsrdaem.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3naiezwev.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3irnihmfj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zfwfkjnt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mrxzzzzc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ohctyejf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fclburkw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jmyqaobc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3anaxrqmm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tgytcbjs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqxfpsh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kdpzxijg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gquqlbkb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3slhoutws.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3crijrsqd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drmjfcqy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oeirjvsg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcflskdv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ennvytxc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvwrkdol.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fkfabsci.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3deuzopkl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fedmbnrh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cdirkhbi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opdhnwpn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jlcffaoq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uomrvtkv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmjwrjkw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ogxtigpf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jhrmaalk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lpumoacm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sujagurx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cnpwbakd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ryudfhmf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3deepktpx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gndwnglj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ejrsbxom.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cryhykur.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3asfhfjeg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3actrjtni.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3elxegujr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3amhdndgq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3afagbwlu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vtjjinyx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tjrklsxa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iflsfnny.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dmlbdszj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mbtlxwso.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fjabqomc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tphmmjbm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmrbgmeg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jzpvpvvg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvharris.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jaynkmxe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3hdzpivdo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xpfzgpxv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bemmkcln.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qukddlsu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ffxcejkf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhvybnfo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgtlomrs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hzjuzqoz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3shtpxykp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gzekohqm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3psdadqnq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qtnmifbp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3iiuctnni.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vjurvgjc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pxngyxtz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3olbignjb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vgdujlhy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yetzcrqb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zmczisrd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jnrtgdgb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pnougyki.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nfeaiewd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3swfhilzo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cthgynve.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gqbjkqdd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3skzsakuz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xusbtszg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fkyxiwlp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rfwulasi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zdtryyfj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hzwfqylm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3keuxdtde.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycbkngla.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frablpoo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3trspdhcu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3llghkmku.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ahhhypmd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zixdbhwd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ekldkujo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qbglzlgh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xypjdmlv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fwmobdgd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xahsxjse.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqukearh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abtdrzom.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bndlomle.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3erusqivg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xliwgbsm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hjiuiqkj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xtypiwwd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ynlghali.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3alwiqtnr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ehfcypzw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yccikfut.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ykvffwqy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pfeskgzv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hnlidpzs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xwvqmfil.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3soixuosh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pwookqnt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rotsbyxn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxvvamag.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3okxksuui.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3goryglgd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrtutryx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cufrtzwk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbpttit.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ybcoghdw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ljycjupi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zzjvfpqd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ztthrfok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kcmqfyah.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3grqyavbz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tfrrndwn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rrcbblog.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bvywnvgm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dsnkcvqy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xtwuplgs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3paaxykzi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fpngxypw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xjgurjbn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jjcpbslz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dmrowxqd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jwirgqad.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3elgsuiiv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tvfcfllq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3asahsxrh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bmftecbw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yhfoawxn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fusrfssm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3asjfexyr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3noxvmczm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sdqtyfgl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3icosssqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytqcrlaw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xgvvmklr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuahjlde.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3urprhrzq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nllmumdi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkkmbkem.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pfbuqgvn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vtyobgro.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xohyfvwm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3spoarqss.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3azuaxoxo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3awshnkqg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zoypnkht.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tfkydixs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gthfkvbu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjggbyo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3drbbwkvn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3prbrctqc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bemkwxpd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nlzdvpmk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ctuprpdq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lrtqnspc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qvqwtehq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3guiisqjf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mgvabhgf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yopohwwb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qkoiqhuw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3smyvdjnw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gernzovn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ubcvhvzl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ivyzzruu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gyqzqmde.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mwvstnko.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3htskffkm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dtfhoovs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3buovgqhk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rdipfstk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bcpldyhz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dfgwctli.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tsjdtuxa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hkdzzxjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kvsgezvh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3khpoesma.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mdqgsxcq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eelsxsum.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gzragdmv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ywfvgsqs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3azaqrzxu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3danesycq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnnxbwlf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vyedaeae.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iugtiqua.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bkdhdcnr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3evmzbhhr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbnfgff.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ajztyliq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3puazrdpu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3inswznmq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rwccxckq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nfvztzaw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tfylumfi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zzazrvko.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mtxtjggm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbhrhgh.html


<!-- 参考信息 -->