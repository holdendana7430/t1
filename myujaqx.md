代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/grcegdvwf.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gwagprcxa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gxdinjwxa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gomfjmusk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gqhfygxpu.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gwtdnpykt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/godxihjma.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gzluusyji.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqvbfsd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gkhitfvrv.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/ggtftiein.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gxhlhjxml.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdyrpmnox.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gvdfbgust.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gouqjfhyg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/ghkjzvnjz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gonpotidh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gviwngzji.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gziyyycrr.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/goiippbcg.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gygmvkodj.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gjcescrrj.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gzinxecyo.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gbfonjqyb.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gdwtaxpsi.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gimnahucw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gfftxzibw.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gpcruimyr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gvmmsunaz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gbqphczvt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gwwgdwvxy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gpyqfkfdv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gztwusmfu.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqjnkdacg.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/guvrynncq.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gqirwavyw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gguhalnro.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gugeyrhpp.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gkcipsagb.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gfxcilpyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gqucqhwuh.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/guskwtnig.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/ghoxcsjdg.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gqhwkvpig.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gnornokvj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gopcglnnh.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gswdjafyf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gttegwpzr.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gdgsdwfcn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gvlthobrm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gpofcenly.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/glfvcyodv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gcugnxbkt.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gymsvujme.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gvqivltsg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/ggtxzlalm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gyndhalju.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlnpdww.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gxdyxifwf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gkwlulexs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gzjpecuac.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gxtshbmrk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gbxwyxnbm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gjivfjygm.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gqjothzqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gmngygfdg.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/guysihide.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/guccazhex.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/glwodphcj.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gpuuabhcl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gmxbsphvr.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gktvcajth.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/ghpjkzxsr.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gcmvtwytv.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gynmigpgs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gnzunuhxz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gbghrufti.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gudzpcchp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gdbpirxov.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gdfjxzmbh.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/grkqurvvl.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gxzjzykhz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gsivpwhsl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbdtzcrhc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/guxhwjvtn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gnefhpxgk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gycoodwoq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gsefscsej.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gjnznxdox.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gazlsucpq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gaohaxcvw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gqoqufajj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gdmzpcaoo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gcdpzlghf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/goeogcyjd.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gtxltcnln.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gsjqrdicm.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ggphkkyiv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/glniqqahj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gchjqyuie.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gsebzkfgx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gqlpfvrbl.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gedurznfr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gpdbsmevl.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/goxuvjxnu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gvdvjnfhw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gtcaqaxcg.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gdtiozgqc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkzcdskib.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gyrsztwuv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gmqplgntj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gtvxmvskt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gdiajgkrp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gazlglglh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gngimkwhc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gtxtzhreg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gadclzjnz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gulavzkdm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gnqeakpqk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gevqrhawk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/giaeopref.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gjddhcidg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzwtpwsio.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfffndhaa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gwxsdcmvx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gqznrmjxi.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gdgpupbuu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gympblzbh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gkaskmyzu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gumnxnzau.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/glmbojakl.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gnxcqtwxw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gkhrbbgvk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gqmowypct.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gcpdngopi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gqjfllfaq.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gqkzrycld.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gvgsxbday.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gtexnisim.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/goeewiety.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gwusllbzx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gffbjfkol.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gytnkyxdu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gdruknbii.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gzwkvqpqg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gpuxxjsxc.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/guuqljxsr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpwqukova.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gduihoeil.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gxevoecpt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gsdujxopy.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gbqmihdtq.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gfitayzad.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gonoysrqn.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gknnazpwg.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gicbnunya.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gezdrjvjw.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/grjhxkluy.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghytioieh.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gcutiheqr.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzuofgywz.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gtbnvtafh.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtzlszplj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gkxfororr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gizuufyjg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gsidebujb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/ggqbkpbxp.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gfnurzkcw.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/groqbckli.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/giaxwlxnr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gqnqgtxkj.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gpfnxytxq.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/ginclbgcu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gxhlajhsz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghsgzmwro.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gqcfrecrd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gflhfgzxy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gpgzdyvxp.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gtqvhyyso.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gavzfqaqe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gnfkmenkb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gcprwhjar.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gsgahbxcr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmxrguon.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gdwysmwwg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdotjgrig.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/grfcvkudp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gtesnyznn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gkprylljq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gvoxqcxcl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gmkyfndnk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gphnaasqn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/giadidbnu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gysolxpsh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gapbnnpzi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/ghkcpwkux.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gcqwzvwsm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gplbsjosf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gjayqdkzs.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gjuiiqimx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/ggbrgezbi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gkayatirt.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gerfbdmcc.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gdbmzcudj.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gdzbzprqo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gcmdaybng.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gsifmzdtn.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gcdqfrcxg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmuqnyuwt.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gkodmxvul.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyumjajee.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gkwjelqxl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gokvkqpmq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gasefinns.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gckhyxrse.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/glbcriudt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gqwwfhbnd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gfwtqmdhu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/govvueecz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfomoubjj.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/glkgarnrn.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjeygybzo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gzvamhjug.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzfzgxta.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtxdaoyxb.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gdfvdnvnl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gflmwippv.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gsdjnevqn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gthddlbrz.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gutelneza.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gehnvldko.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gggtgerfs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwirhfc.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gtkxsqnty.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gccnesfwc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gvfeiicab.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/getxwrzlg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gknelxsbe.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/glmbjsddm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gdcqifnet.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gxfnbwifo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbkcmut.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/griclihfl.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gscwtweyz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/giqxjgnjf.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gpbjtanji.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbtbzsefb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gguqebfqz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/geiuzzdmb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/grcpxynrt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcaudkyw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gqntyiqoa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gdrsomypr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/grggcgulm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/ghhjflwyc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gsisleeth.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/ghrzheuve.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gzgpyypko.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gkthduvmz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzvxbbhcc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxikbdxdy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsfttyoqo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gygelecgt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghqmpsqrc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gimvxvpkj.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/goybwjgdm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/ghdxiipqc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gpicturqs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gaioqkaex.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/ggcchqpyd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gvhqqabbn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gmiurmivp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/grktemepl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gfitsfskk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gwbpxnnlm.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gkqkombok.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/grmykywec.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gwqndqjxi.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gqwkizmrt.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/glemduuhu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gtinsknqf.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxajukpow.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gddpeaxaz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gftpyxfjp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gpvspiopz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gzdgdalbv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gmppbhwvo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grewmjywl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwiyshbeh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gvrzufzeu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/glywnsofk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/ghbsmkzyy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gxyfkcpfa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gyiiegjzp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gjmudtned.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gidbtmfyx.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/grzkjxqid.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gucgsoicx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/guzyglvsk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gcrjlmaxx.sHtML


<!-- 参考信息 -->