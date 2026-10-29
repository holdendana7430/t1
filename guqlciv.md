代发 wailian999

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gbkujtgfb.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/grxigfyux.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/glfrnanoj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gjwghvfjq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gzvywipez.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gjxbdksey.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/grjhegzea.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gvkgdrbir.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gxhhmmdwv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gwjapsare.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/ggdufkvbc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gvbjahovw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gijkyelmk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gpckikbhh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gzlynspgk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/giwgptsxm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gyjnhvcyb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gnbcpdfhh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gmnevpzpy.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gmusawjkt.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glwfiqbvx.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfrngfxvp.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gvornmdvx.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/golgweltn.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gvoqzrmwc.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gtdtilean.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gjievbrqv.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/glwwuuuxp.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkfdemjja.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gxfljyglu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/graozbakz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gytmecxxv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gwpnxlumd.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gwloymvqq.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gqtvkdimw.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gsowfqbak.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gcqmgfcti.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gyzkexbdf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gckujyoey.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gnuderizy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gjikndvyt.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gqhorvahy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gxeahamlt.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gyuonadga.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/glfoyouru.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmioaadwh.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gilqlgdyn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gafomlaml.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwgtddiij.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/glbskugvp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gtsahcrcq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/glixpvfuc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpuclnghj.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gjfkbpiik.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gfawvqayt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gyvmdtwpp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gfdxpebxz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/georukssr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/grmhentfp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gbyawcdvi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gledmoiac.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gogniktac.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmvwivik.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gnifghibw.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/geqjxtlbm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gsxbxbuat.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gebrlghxm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gweokabhw.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gtgicrbcd.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gdpwdenyt.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gflripadk.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gbbtfooht.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gmhjexztg.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gqvfxryjr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gzccyogwd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/guwhnbcld.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpsldoyyr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/givptphbq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gbzhpjwtm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtmloshzr.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gfxzqklkh.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gsvfkspbb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gwbvvdtfi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gcjgvnfaw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gikxgfqlq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/guyqafmid.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/grsocvrhn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gaxhsxgcx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gqnapcnef.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gevbrwpdq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhzqnhda.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gslrcqvcf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gdkhmijaq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gwtnzyeli.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gxfweiflg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gktczoxpo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/glyaytozj.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/grxaucitv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghirfrkqs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gilklbknv.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gdbnajlqw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvjzoal.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/glsmnxgaq.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ggjdrnjpn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gyxwllgdl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gvzarbjxg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/ghgcwqnck.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gbrdhtqkt.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gbbnmpswm.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gsneeeycg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gvgcrvlzr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gllbqqotw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gctognzfw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gumqraoni.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/glfdcwffe.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/guhbsxllu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/glganaeon.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gbyvucifw.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gtnfkglsg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gtibqkymv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqcglhcvn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gcdhstvom.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gqbecnjnu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gciufiplc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gwywrpiii.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gxtscyfpj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gygklnvbs.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gvwnyfyxa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/ggdqdccam.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gvtgxrakf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gkgtnodiy.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gwuytjcca.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gshrjycka.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gjtvktpog.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gzbmrfuux.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gehkbwwuo.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gnnvfrfwo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gdcydqcwp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gqyangfav.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gytkcxsfg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gpudbiyte.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gymfrfvmy.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/grhgdqfiw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gjpdscyji.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/glszijwxy.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gdbgqenbg.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwsijpwrn.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gkomzfktr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/ggmjeacek.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gnwliisdl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gphpbltyv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfmscxnki.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gnstiovuc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/giwrihjgr.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gwkvwbook.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gyaxnpclc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gccbqvhiz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzbgakclv.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gpdidkwdl.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gyomzsryg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghpilfsyz.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gioqpyfki.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gshlkzzwx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gtbtfiacb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gkhqeueus.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/ggqydigak.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gyaaofsga.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gqlpwykgh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gjzoycvjg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gbsyhrhgh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gzzrhzjwt.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gifvmnime.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gdinkhidu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gabfgmhpm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/geiwpwsvx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjugehwcu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwkubrmec.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwysilpz.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/grxhtmkvr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gdqlbvczf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/goignyuwj.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gnwkqgddb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gpregqgaw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/goqwhgcco.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gdfuaeddp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gixjavzbl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gbhvfbvcr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gcmodyito.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gxxxiqiwd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/ghaarygue.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gwfiuhktz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gdaitkrcu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/goutxjdmf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gvyepkmyc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/geutuplhk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrlhtkv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gnkymwhpc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/glrikdjax.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gyuasuspn.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/grjzmrlsj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gukpgzwrp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/giycttefv.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gowuextic.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gwujknxfw.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gqivbvtio.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gkytsebfd.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghbwdvceq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gysfxwgfk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geihailfx.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gkmdvjtwr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghklpjaok.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gciefduqw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gfvlqhmqf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gtynioccq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gkablscmr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gpwwylyin.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/ggrikipfb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gjozdcwhv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gocddrrvl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkhgjfkuq.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/guhpxpjsd.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gohttwgjx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gvansdyel.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gbydqheot.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ggogvszcw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gjatxnjkr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gwymtqrtr.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gynjpyunr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gfuntqmpz.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gdexnftyl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gxwdekwbi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gcajdsqnp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gqcjhgccd.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gfplanqbx.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/getqthkyx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/ghomdpkzd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gtecrlnkl.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gkyvzegfm.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gjxrsjvqg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/grmqwkzlt.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gfuhuazyt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gguuxqmnl.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gwheyjtdu.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbqubmlbo.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/goghfazak.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gzmnqrruw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzkepdpsq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/grbkbyhwp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gdojmshhk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gsyclkplu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gxrsuqehg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gfoxgdqis.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gcxhtllcq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gsopyfzyk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gxqrezwtx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gndvifkgv.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/govhwaxze.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gqyzxcdwg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gvwgyecat.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpyxawnmh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfwhvojkn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzumvywkx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gxcomlapf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfgiomvyi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtibyaqr.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gdwcdbdfa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gsqnfflpd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gashvenrj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gjxxiucnk.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gitlpcrad.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gtvwwqklj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/ggohfqynz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gushvguhs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gjyhqjvpf.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gvsqmjbyn.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gvmrgujqg.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gzmklzlvy.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/glynpgoos.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gnxmtxyix.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gmjiyrzpz.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/grtvjnqkm.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gvlngzaxw.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gijgmtrmw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/goqbxkfzf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/goewocmjo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gxqahxvzf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gslwjromh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gwpbhjaci.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gwzxgwjvu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gceuvbccz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gwftdeqpo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gjvbbvmda.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gtgcgyapk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gwlpueppt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gtognrger.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gsevimllt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gcsaxkjtk.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gmjtjatvh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gglajoehg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gjsoscjqr.sHtML


<!-- 参考信息 -->