代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gcwjlvkdu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gujtpfsvf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gpjfkuxxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gbfdnmkgg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gygxmbmuy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gcxnilcew.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/glzauuixq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/garmtwqbs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ggbllrlwp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwubqmoqr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ghiuxfpbf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcjtmiybd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ggoolyhvb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gtvebojvf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzsmbpxwx.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/ggsvbrywv.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gukblxcgv.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtxlsylby.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/ghsewavqb.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/guheqkxbg.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gghwjykfw.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/guioashkg.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gkiravxsi.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gjobrqyvk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gttppzsob.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gjzmuetzq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/guabbitkt.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gobutspnw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ghxfgppgq.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gbhbdumpd.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/grcmucxcr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/glbxxcews.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggyotfqna.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gctvpcxuq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gczwahdat.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gdhmwyfcq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gnzgtnxwr.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxdugpr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gurbyyvmh.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gmdwkodgl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gzncdrpkv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gttmvxthe.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gugxnkqvn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gdtqhnyqx.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gneibryfs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gmbducftz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gtdswqooj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gxyntvjew.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbfaeudie.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gsmsvcqgl.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/grrghwumf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gqjsgaymq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gsrzdjpbb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gkpsmkvgy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gonamynul.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gepurfshd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gwkmbpauu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/goopzkoqt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gkpprsaik.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gulyzmtml.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gmmovvrgi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gusnlhxsb.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gbioihxgd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gusfditcx.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gjohklzwr.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gxtfzjhub.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnvfycxtr.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gyqxlnlhf.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/ghahmnvfz.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/grpeffbiz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gqwaquwqt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gehnwpbvv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/goiigxjko.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gukzqdelg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gddzbdknu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwayxdssj.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/ggfnbucre.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gdkhjqieg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gfpzpppwz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gtajjntig.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gpevmkuxm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gugpmxbck.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gluwbphsg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/ghkwshimi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gqgohazop.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gkpbkrepy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/glkxxvbhj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/ggryfkfmv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gvcbjkoww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzyppytlr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqsdgzsus.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gouveeiad.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gyqfldwhm.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gvxpnodgb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gdnicccwa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqbldanfy.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gjkkmxycn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/glgxfzkhc.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gagvckoof.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gntkjylqt.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gtjyapput.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/giiziyelp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gmnnhzhuo.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gnuvpfjbz.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/glnizyvqo.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gtjihuakt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gbpgqdday.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gwyfxdgzs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/glxfzjsuu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gnagzknoq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gtstojvem.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/glhskcxwt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gnvjkiitp.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gluttegup.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gchnrjqep.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gporunhkk.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gqoyjgbdo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gjryblzjr.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gvrwpapbe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gthhhpkmh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/grhjxyxkm.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gefkpyapp.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gelavzvht.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/giqwstmhy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gwfptgsyd.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/goicznzkb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gnqdcraut.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gunfdksyv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gwgeemjdz.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/grgmusnky.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/ganvwsenr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gapaerybi.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gysxmrium.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/grntralhd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/ggptpmcom.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gsqddwvcw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gqgvrcgjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gpmefmtoa.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gehuzwark.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gsriawctv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/guyywvwbd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gbwiqguuc.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gqxlcazfi.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gngpokglp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/goeubolfz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gltfqupyw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gkjjqffjm.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gdhknrgwx.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gyjroftwd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/ghscztljg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gzpezlubl.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gxvpctcmq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gwhmglluh.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gexfzgzqi.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gyuyxuady.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gqrnhrmbl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfmdxlldv.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gvtlguigg.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gwvxyqjcn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gxbfslvdg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/ggxfohisu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gvciljwfb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/getppmdlc.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/guyyrfcek.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gaixlagys.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/giyhmlxll.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gmwijysxg.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gmbjinpaz.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gfhnbqunh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gdgtpluzi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnaorzobe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gayaqowme.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gjxlbfwjd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gourfrwxh.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gztmurtgv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gkobivfbx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/giumevbva.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gkbctxvbq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gyaeemubn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdvapjam.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gmozioamb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzrhfmqif.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/grrkwjwnp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/guzikidwl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gsfjxolhv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gstdgsljj.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/glqnfpziq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gbauaqayu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gqkjptbus.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/ggyblgofa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gnrwcglya.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpakxuiwc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gvjcgjyqu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gvbthyhfe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gijssgabi.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gmmgobqxr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/ghalibxbd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmzvbudfy.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gtdljabwc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gymuglrqn.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gmspfvldn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gdqvmplid.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gqdzozjpe.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gqpkcvfpz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggzqluwvf.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gznrttule.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzppdaswt.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gtkkigypl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gpuhancib.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gruluhqoo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/guywfafpp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gfppbpxnx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gjyltmddn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gwumlcozf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/guttdoibd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwpprqlru.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gjzgaiosx.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gbqnvgdub.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gkvhnhqkw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/giidwbmod.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gungixmsa.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/glxydkhxe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/glhqzyioo.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gmucujqga.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gkbpoqtov.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gxhkbpyel.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gfgmpnkgf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gicbwlyic.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gfelvxpsb.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxwliemhn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwxnskrvh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/ghnqhpgsb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/galduvcdu.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gifgwxfsf.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/grviqqwyc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gopbqdvmr.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gflbpuazf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gplygexrw.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/giukskpgq.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grmvufxab.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gdaahyjrp.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gkcezippx.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gtvigyurd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gvgplmyoa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gjrcottft.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gnysflxln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/geigkuqjf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gppthkglr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gzrqqxfhp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gliqwjuna.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdkcokhcy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gnyfcphlz.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gvyuxkpuq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gknxtejnx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gacjtrrsb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/giikhptxt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gemqakbuv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghxyqukay.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrrnjjti.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdszcauvh.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdmyimvur.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/grznwqsnq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gunmlgfrg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmawgbxnk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gfoipumnd.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/ggkjubciq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gkxxfjams.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gxuwkeyjr.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/glshoppvp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gsosvgvfg.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gtqecvtqq.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/ginpvygqk.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/geufimida.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/goqdqzvyg.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gurpmvnzx.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gzlfmxpwf.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gcihkukgj.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gzprqotsj.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gbogchwhk.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gakbsucee.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcemttfe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gsgrtunww.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ghmtluxiu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/ggeevdlzg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/glrjzqtyu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/glorqmexf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/ggymzyojx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gydmpgxvf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gslpuyaod.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gaifrffbd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gnzftwzdb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gnyleomwg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gdvfztbiw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ggaexiqyo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gugrtszbt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gybhmpbgi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gfmkkuccn.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gnirlyzna.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/guhzpriec.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gchiajpal.sHtML


<!-- 参考信息 -->