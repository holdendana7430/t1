代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mfgasccq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mbjzjpvy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fuyijiuc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iixkvxsb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3maihixxq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fqjwlviu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3icqfmnpl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjpqxz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3titbkicr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3amulzocz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lqeroash.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3miadpolt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qcpyvwid.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mcsxghta.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fyxhradb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dmayrrih.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3poliujig.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3puiqkoyc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iilvzrii.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cpwttnrw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3unoaunsh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mqxcczvk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tteptucc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rjuidkzi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjzbmgl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3chuftcaf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fyninibj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rzqyswzf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eaqyqpsa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gmxbaeuj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uveebhqg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3pbeomstr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nqfsycgb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uvnbcftd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fxstzxqx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ckufgecr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3umaouare.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3llykwrdc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qkvqywgg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rniftcho.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jatyqbaz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ohujqmvw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ewsmuceh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wwqinwol.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pcmkhguz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zusaqrla.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lmbpgbbl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hbqekurh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lsegxnap.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gbrfwopz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3enhbfpph.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ddxgkpcj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dgoettgr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ysyfbpqu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqizphs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ifjleonj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hjalxkzd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3tdiaikdd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3coghiuoi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3czrsugte.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wyyypawi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zywruohk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3aihvuhfk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3opzamfva.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3amyffdiv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xapvnogn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qvjdmhgs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wdzmtuml.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3umtlghtz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sewdgogy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mvbtxpsu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qcaklfvx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yqinrihv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qnfapady.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ispvwmft.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dcgwwokw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3pmmrzczh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zkvcktlu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aivxxohj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mbnqrazh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ihnghilc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kahlncnp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mmjpwjlf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wpfpnfte.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qylwksxm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qtkctpge.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ruzborlx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hjpkjkin.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vyawkqla.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rodaltsi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ueuirqdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ushkygfw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iasvoyha.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3grlhwwig.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lcvnwynn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3elfwjdci.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iqgvhxoi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3aqetkgsh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3khrfbkhh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pxmqfuws.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pqhzybxb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jlcvlkne.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3szrsgpmf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhakoqyc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jirlziba.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycglhown.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mkvcvlxu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3uyjfomcj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ostgizio.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nsotwdlp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3juqwmros.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlkylufq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uyxttrxj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cdcuedat.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aeslgjzi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3beylrzfk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pgtyhbdm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nsrwbuob.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzycgjnw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hxixsmew.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3prhpfvtz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mldgzpwe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sojyaymr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fdlxxrvj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3eshacxml.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3odvpdqik.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgfjxbya.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wiwwzgos.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3obhtctqr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hjowxxzw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rewmanix.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rjtgfppe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ufcvgyxj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vtnqyrvi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3efezhdiy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3znwfyczy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mdpctzzu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qaoldnab.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3msatkfmt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gdjqwhls.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjsoenen.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3aovdtqfg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3unbpabfo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vsxlfnmv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kkfvzihl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3uwfxhmcu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tnfthjeb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zvnubzyj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3pvhoectu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3izcozlzj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ykbtjgty.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rmbtiybm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zpdhoyud.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwrokhsx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dnrkumob.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3tgfvwlfd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tgoghwby.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qorpwqdr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ikmdxrut.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bncnfhyb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gojyihlo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ytxbzcro.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3iiinqvin.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zypuaajr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ctsbfcre.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lqhxfdil.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3stkotqsm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ruryukpn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kyvyhqmn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qcbfmkcm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqjlvshc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ojbxrwkh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3usouqtus.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mmqgasuh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3odcsloyo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zpsheduh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cfihplpy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wepcnfcv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cazoyxas.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3utuwiphy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zdusvnro.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qfthtlwl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jkwkvrmg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3tnktbdll.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yrzbxuom.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lhzndllj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3auwvxtby.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3iwsvrdog.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3igqbynvy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jjdahitq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bskxycmt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zhzozozn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3peqvplsn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cfxhwdgb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3trclznto.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ictugwkx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kigwzbtm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dmhpfcxl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jgxmqxpm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mfpiywnk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysqexszf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmnxmwej.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vfdqodlv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hlulfoea.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3retplctv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vojpbibk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3yatmdidc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3koqtbxbw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fshgmzxg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjbbcea.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lecxqlte.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cdikmggs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lavmndws.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofreyzvs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbxlgcf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wwhrtgxp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3owlbkwyf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isnolqpn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lekoxaef.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dcncytcf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wulzgusp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rvnqvzkl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uebejmva.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3udscjkex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpuetxmj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gkltltlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3haxnzfbx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lvvrcycm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zcejlcgz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nkwtyzkq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jtiniuaa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zemawxvs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qqjulwtq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bjqstllq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3midlhluv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wweorvpr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ifdokoge.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yozlznmz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ynojvcqo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qwovraso.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fzzemava.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqvexqk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ojwzkznd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3sxekycvt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dwxlwymf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ksrczaia.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3arczanqz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vpvczcuh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ubggawoe.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3atcjpiik.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xvhcmmrz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jjrpxzse.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fqptbpyd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uemaecjv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fmcadbvw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3agrzhqkg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3scvexskn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bzffosix.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aoazlied.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cycijabo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gkamcddo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3egzvjabb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dyyjnupl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3srkrnppv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rgomeoef.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3omzamyes.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nqdzmqyh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3axhobyca.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3falepjsh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3grwcjqcs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xkbymthd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3axduattf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lkjnskhp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kolmhmnn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hdposvdb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ygsnoybq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fwgppwyi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pzoqldxn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qryymhog.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwibboxh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jjohygem.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oqnjmapv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qcjclsny.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lmjttbtr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sioiggrh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3reycckdg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wsohylbh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ashujwos.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3izsbulab.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ttkunbph.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bdfutzmd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hvmgobsy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hexevypm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pxpiqaok.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ukduxodw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vilgiegi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3plgfuvzx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dseptsdq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dbwbwpdj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pffjujul.html


<!-- 参考信息 -->