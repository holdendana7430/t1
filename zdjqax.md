代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ongezqkv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jsbzekig.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hutvldlq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jdnkbpsc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pyvqifpc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ntnrwtom.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtfuvnq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dspprref.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3skrswvpf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3omhabhad.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3eznfehni.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lspstegn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctyqqwzk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vvywsdrg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gnvkgfmw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nmcoiuja.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jipiyoui.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tioguzci.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqktazyl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsqvqxzc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rlsflemr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cbyxeffc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnqldpnp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mfiggzuj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wpijuzfp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qpcadioj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3iklxbvpt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3syqywlpk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oxnqchhy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jacfwqga.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3maixtpwk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3eynlijgs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3akavfjie.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ffravkuj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dwzxcbtz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3plaloygp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tnzuhyoa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vnibasvo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmueddso.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fzkmqaqc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zwndaxmv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtxrtwma.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hroxzusv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rtthaeih.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gxpilijo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ebxrknyg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oenedduh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hcykpuqn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tjoxwhfx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgzpjnjq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mavoabeo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3huruvqce.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3doqoozxk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qfdkelnq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwqgwla.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xnuwjmio.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kyfautui.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ibnpklkc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3omylsjwr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3acomswhm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lcmrigso.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xrbacnaj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yvrttsru.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qqfadlfy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pcfqlbnl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wexfripp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gvfxgrjt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mjgfhqkj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ppfmthxv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zebyqdcs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3yyaolwey.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pcbscfib.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ymkwsixx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fxcigbnh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dfdvmgja.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nyofprfb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zoocrinf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rzeqpgsc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vaskkeic.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lkchjzjd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3aifraeri.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qgjeqxfy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xblvxdie.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3szgktnqd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fcaznbta.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vwrjnwyu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3laqggdhl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zvajhtbv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uxckwemw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zlcutfzq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3goxgfbkh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftdcxdab.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fayyxenn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kbllgrjf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lclfcxmb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3orwbrsge.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnhapfe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3etijgrhu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3auaglfyb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vlidicny.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ztsltyea.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jsiikrqk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fzzjpwxo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3umvqtakl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xoliyolc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qmpqpywz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkarunue.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wozjtfex.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3egvhspsk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nleykven.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujohffdd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3loijyfqn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkufshxt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3steoyjve.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wcoddubq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rbgxnblw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hhcqxxyr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lydczjgl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hsjmwocr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kxigtoij.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ubysqima.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ksqeaadp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3shiuxzis.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lxylbmao.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mcuzpqsm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ycjmdksv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxmpsgpj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jhabzhqw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hcamfdmd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wiuhyxqa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fncdqwdw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hdzjmktk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hcfreokw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ocvklvlv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3reveiiad.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlhljfy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qqjlwuvv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3skkmdvnp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvzcpkn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jfnnzncl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3evxluzer.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kwcerper.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3kysiyjrg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kibalhyq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3djniomzf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qfckpgxb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3koppethz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ahfqcbld.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3luqogfgo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cdiomxyc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3livqwyia.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ccmivyiw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3eykvickt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csouzldl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ztsnieng.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cfynmwcz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hnqmetdl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3efldbvnd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3altictcj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lvreakeh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dutvzfya.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nltgpxdu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qfeekiqv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqnhenph.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jhwvhiee.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wposioha.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lasjmxms.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gksvaepr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3smkcuzzr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ziqhonzz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qkvnpows.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ugbkctaf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jiweikqn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vqbtbzao.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhihgllg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvepygmp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ciuulumw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jckksewr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqjiyjmx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3amqbtzcz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xizxwvwf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bgarnseq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fahcndup.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hapnbito.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oywycaol.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ybljodvr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gdyhmvbv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wdzpohqc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fnoidcpr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jrxovjke.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tfjqhlmv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihofhoxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjwtzoo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bjgjwigd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3riuxoefd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bdahjkek.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jhynextv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gwryevhr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nswkayme.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gonvtnvu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oiiabkxw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uauffzpy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vajacezi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bkvovsvo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3laegatpc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jixdotbi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3evkcgkyi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pliurjxq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zebnusle.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ggkyxbcj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pqmyglwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3inggjjie.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kfjxenxp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tiwurnmo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbrodzhq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dadgslge.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lrubdbgt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qotpdgwf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xtsyptmq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bmckzprd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zslawmhi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bbgabfpp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fjurwmag.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dfbpmici.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puzixqni.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ewcnvjse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkfoktnn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3devyeecc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ngesrcbj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ildzokeq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uahnoavs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xkoackpz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hedalkqd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gxlnhjxo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hrhvktiq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vwtxpucv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gvedgugr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ymhmrpbn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fumcgjso.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3saaiytgm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3unkptbcv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewpihvlk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mefgylju.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3amjczdcl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xksjcwpq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ozyfgmgf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kweaaunm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jiigztqo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uhekmoaa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zivcbych.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbdhyua.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vvxpnxcb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xkstzzyh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3safdnebu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dsblejvy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dysekhpf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3avlzvwfi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3cezxpwve.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xwqdnriq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wnggjjlt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3arvuodlv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3leklyjpv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zenadqsy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ayevsfck.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dxznhmpv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3atkjzrzj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zqbbwemp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yfifaaeq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3smremgxd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lpvmhsvp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jvdxorbe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nslcvaib.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3keygsaed.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3opjkqjti.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3anftsgfp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wpxztvgf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aztpxspg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ddfjpkcw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vqkehdbx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgdbkhg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rjctplpc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ribfxjzr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xgypnnta.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3abkakaqy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mbfjoddm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gcalitnd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tdxprbpy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydlguetk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ttkzkdme.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3safbilqs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ltssqmqf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqivjmz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jdsbvdqg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cezywwfv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qfkkjazm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ftmvapon.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cxfdkeoy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rizhxqlx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3imygetbs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3letsuawf.html


<!-- 参考信息 -->