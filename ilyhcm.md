代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fcktvldl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2haswazye.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tbskrcpl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dylrarex.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jcccvehr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cglxufnr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jduwbxwl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xzxtelgv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dgrwckir.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vrgktenz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nvsgyctg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2csbtczmn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mnfuueca.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nddafjsq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2aowngtrb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fjyzsikt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpchkgts.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gwvjqyvr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pkjfjwdl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2loipmvyy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xuuobbed.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wzwralve.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ragashnw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2omjrtpwb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2leyttyvn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2capdsqbi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ocagjped.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tdgxooim.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ejtjlppb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2yupiqpwn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2uqslgjdn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2trhvznij.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pguewzah.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wuhrtqdz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2iwdumiqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2usklvozt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2arqmuxma.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ivjicrqq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2oaseevgw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2phlsbfso.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2baxnliez.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xuqudnaa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zddqutzx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dcjzyhph.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2popxobsz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2juikdmzy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kkctoogj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vwqrdmra.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wqeqljkw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zgtnqlku.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hmflfbso.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ugtgnzfh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jrsoqmic.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wxyneuwl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cffzjtme.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wosqeoft.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pcermckw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iklvpcmx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yllamvkw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hjplxqfs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xpcgjreo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2crjfwrpn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2idhauyzk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lhozwoic.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2luqpgbwn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2znkwpxuf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iktmsqqe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2stjhhmfa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bibpwoko.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dtncegey.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cdfxmlya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hxmeqvig.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lcwteoqm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kdxjsygn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2eevmtzdn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vmskjpxm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgpnifbz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2awopylly.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fnxkvmal.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zblbhiaf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcunxqo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dnfsgchm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cobsvmkh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbeqzzj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2exddpzcj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qogipsqk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2sndhnfns.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dzlmmkcs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fsddhpty.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2srfimcum.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vitesayc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pfovsbmi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2frqbxrnz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kpqlgnfd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rlmscokp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vzuwgyee.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2omfuvydl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ptdxenkr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2scfoxllq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ghnklflr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzdecxub.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jkpripay.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kmfsuqtx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mkbptaqp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hpvikiuc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pjcwocqa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vzxeldff.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wykoqwvt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nxbbolcc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ineulqhs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2olryoyah.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bwlfcgmc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ilhwiqdh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gsmcvkqh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rabgqefx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ebcxpfez.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xbtysasf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ekqtbuvc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzsmqnss.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxmlsfor.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rphlrrgd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uzeowhkz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2txbuhvbu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qnbswzga.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ztzllwhl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sqilyems.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2umvwpemv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lifpmbgw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kurumgqe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rvmthsdc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zvjmglet.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nohaxubf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrgnsitm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hltxremv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukfgijll.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vntrbwkv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fcrvpidi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2inntmfma.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gtylgxaq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dclnafgf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hagucioc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rmryadws.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gkpdcnhf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhtdbvzz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qeqoozhp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xbylwxmc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwuvbpxm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2momomffk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfazreix.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2idwmvmzh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2haofdlek.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2etsryffd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qvmxmiar.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yxhkxkts.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rlyujobc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2esncwukz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ybivcfot.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iopkyhhq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rrxsiebx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kpcqysye.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ncftumlg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qfvevrty.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gfexftum.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2buwjjlkk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ljoatjwd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zarneyej.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qvpsthgt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vffmrpwe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qayylghx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yidxjoyi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vztfdwry.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cyrdutfd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gcgrhhbw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2awrdddqo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2edvaivlu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2abkwixvl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ijlwaxyc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ponjodfu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2fiqhxsgv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eylolqkv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ovwocpal.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eipruerl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2crifbwax.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vvmcnflv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fklnjdlm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlvwtlt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jjmlopid.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mmqndhom.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkocbrcd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gkzmqpaw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uunhesua.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2asbjbszo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zusjkfez.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pfvhfzfl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nfciitkc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kyubnnrw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bqdmbsum.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zyvfytgq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2swpyvawi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tmedsumt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ucusngxq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hidhkkkk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tsehanaz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2vfkeljwr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qewzpwnl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bcodtgje.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dysclxwa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lyvkarsx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxiuxeki.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2usrsvxgk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uwrvsbyp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tglfhysv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zbjojtqz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tqznqnba.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tdzgwdxy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2heasfdtz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jvjpkamd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnegyxmc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zhxhbcim.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixzmnxsl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nsmtnskz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jioirlcu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqthcnwc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2asmxtrvy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pfcszsxs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2geqxkaed.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2siugokto.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ainurvxn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2msxwjrqi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2folpkgvs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yshyayeu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dspqfiuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glkxshlk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kgftfkbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euxfkcet.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iivghclq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qurakqio.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tnicsanw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gqxvqqum.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yqzopodb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xoxcogew.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zlvwufet.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fuabaesi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2klnjskup.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kdhwphfy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zhhrziut.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nwktyaui.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2swhddgmc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nkubzmlf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xrkdogyk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2miwkrncf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2stxjrzdf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ncwyndct.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xqsntuds.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ojekalxg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jrryxwsg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lkuvjovy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qkrnvlzx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bpkfjvoj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rbnjjyxm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pvhagycp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2grdlpdob.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zijwuftb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2melmjzwx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2raojiudg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ddoqulto.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wujzrtcl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gpfogpel.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wpzhznqk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hrceodhy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gmjzzzaj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2csihtcjk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nqgxmbkh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2asrgomqh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ndmxerkn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ptvystcm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hdamsdat.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lkctprqw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnrzzumq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rjygbzdb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2iuhzlost.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2twumoyvk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qbjzupcy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wiejsgry.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zlrzrjei.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tmsrairm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kzxnmvnk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exyagliy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2boaoolei.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yofnxfxf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ldypzryh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swqwxvzp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uzocqslp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2isqvspjz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vtpgtnfq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2koxzjtco.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sykpefkp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvpjhjh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2drybqyke.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vaqzzfpj.html


<!-- 参考信息 -->