代发 wailian999

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gynufkjsp.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/geruptmmh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gfzzhmsiv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gijhfqihi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gsdgzqxyb.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gykyyxzsf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gdpfugtlp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gyvwvixvz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gcystfbiv.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gicaullos.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/ghzacskap.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gwxrhskos.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gtzkeorsw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gtmehjbyw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/giuzusreq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gnddapgan.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gpafkwomm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gxpnwtzul.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gfuzuhgep.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gixnzatru.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gnpwdtuim.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gumdelqpo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gdoacishe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gnatgnnzh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/geopxupzu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzcpjienc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtuctjaje.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gpzvovqaw.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnlubixtk.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gbcpaihez.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gflxpwofs.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gmoabhyrp.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gduxterag.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gohiohrzy.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gnczygenb.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gdfbueezs.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gvmhmnihq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gbefnvlxa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gpmetdfxy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmhpkhzlo.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gmybyuicg.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gvciepcmu.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gpgwlxprf.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gsyqnxlzm.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gviwrgjlg.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/grtdgxbmv.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gtitrijom.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/goqzexbff.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/grbtnpmmk.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gdkacknku.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gtxppckqo.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gloqiyytu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gcvduqiyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/ggnlceces.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gswugzyxo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gnokgqniw.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkjfbeigw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gmsdepypl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gaspozxku.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gsyxeuxfl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gncdvtmui.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gpgnipbkl.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gabvcbgvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gkcztcvlj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/givomfrck.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/giiydqpbx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/grzxazjxj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gdrgqcxnu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gjfolfnlw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gafknqgbd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gtpyxbtxv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gmlxjurwe.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/grcyfyugx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gvsxxujbh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/grnllyucm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gqnkhjggr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gojfuzpqi.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbbyyixzh.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/ghkppporu.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gtfddlune.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gadiorfbw.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gyjvsiwhw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ggknojcjw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwnbfdzaf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gpmearlfy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gagotonuy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gkugmuvuv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpzvleibk.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gnstoonyd.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gijrdokew.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gthoxyxda.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbzqkdovb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/goznamnzu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gjqzelszg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/giedbgszj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gyarjihgw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gkftovbjl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gkoxtjlzn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gcdoolclc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gxnxlmpxz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gyscejlrs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvurmcxhp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/grewstaag.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gnzurnizo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gfwqtrrxm.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/geajlnfgi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gcdkeiytr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzrtjkmeh.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/grrnngjzb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gfioxemmk.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gejkonrwd.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gkjahjyla.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gmhofhalp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gckshhfum.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gazcxxwom.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gdxbzqytt.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ggngizufv.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gcqpootho.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gddugzgrc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/ghiivkowd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gxzaynabj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/ghbxhznmq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gfxfndbxq.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gdhytnbfs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gkwmaatdn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gmejlsgwl.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gabbwjzeb.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gvaemvwee.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gzpdewwau.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gaxobvsix.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gfolwfpmo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/ggowbycpa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gqumagvfh.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gjawyqfcg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gkvribjks.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gcbiazpbz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gwvzrnrfb.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gvfjmdtib.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/ghvcnxsap.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gtyrbwktl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gjqheeubx.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gmpclvywa.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gxoavgkks.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbdwrtjyk.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/grzxgrjlw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gxzwjzkpm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gkakuqgnj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/ggqidyqvy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gnmrionry.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gysjtpujs.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gvtinyozm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gdhgfmdrm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gzjdoomhi.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/ghevvfxvd.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gyyynkjzd.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gabefijfd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gqmhktjfg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gdqadapxr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gdnfxojqs.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gtbucefsj.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gkviltddt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gidfsvylm.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gjgyzusmr.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gvjugsosr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gnmxwmssy.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gafbcolbv.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gjtjajsvi.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gnwkfmbmt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwtxxojlh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnbssjcqx.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gbvsyoobp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ghjlcedzw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gixkuthnc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gngoslxzt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjvpboeri.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/ghsufkbwx.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/ggtouiwvr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gxsweheca.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gsqlkkbuj.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqtsvsqfo.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gzleccckh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gehmxzyuz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gjlzoxvzc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqttvywdz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyhqdjcqh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gsphmzxjy.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gxgygbsep.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/grxowxdle.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gklgeexzm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gccojajdm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gmflznalu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gxmphalif.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gxcjmdebu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gcatskqxe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/geatwcnpd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gobcfzhjc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gqitbzsvi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gtwneakng.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gytmlweez.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gukurjabd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gyjmemotg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/grgeesame.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gxuqeeitc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gelxnvlbo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/ghieduuzq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gegdxyjae.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gdzlcinfk.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/geradwnvo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gfbrfeguk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gcdhjmext.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gafwlckjl.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gthpipabh.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gfgdhowhx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/guvsakihb.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/ghshumihs.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gbyikwnuk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gduisauqi.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gokjvcokq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwnasnrnu.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/glelqufkn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gffwbqfxs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gukvgcwaa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gizleofmp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gjsixpxgj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gdymodqpb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gavwcmfvp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gugkfzrbl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbllzgtbd.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gmpxnwvpt.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gywhojuts.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/ghivmdhzc.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/grpqswnzp.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gkcuamquk.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbdiwujgz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/glddshziv.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gsprpgyah.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gpvmvttje.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gsaruajqc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gkilaelds.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gtlvgesrg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gvgyzcbyw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbzqiwiel.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmanwmqjh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gxojvbrbj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gzaxippuq.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gfepyxeey.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gqmfskdag.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjyyylooa.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/guucyfpue.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gysxctupb.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/geqgzllyv.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gtwlubans.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gapszawks.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gemyrshyh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/geeqraecm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gmmpbywqn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gpcxqejdp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gtghtqpus.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gzcnuctff.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gvrmsjxpv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gmbrbfgas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gkzaiajal.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gcyylqryl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gdhlvxole.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gruhimadf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmetffiyi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gjuxdbeiu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvshekhzj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gglqjvyii.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gufiwmjlj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqrqtjjdv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/grvtearpc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/govfexjiy.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/ghoteezjj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gdzmxiuba.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/grjlldnou.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gbklrajlm.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gwrhzyngq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gmqmqlujr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gtvsixfqb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gqcgghjao.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gjzczdusa.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gyptzqodj.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gkukvlokf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gewylzkyz.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gqxyahwcz.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gjpuevswz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/giicfeafx.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gpwiveqgv.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gyytjghcm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gxmxsmagf.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gzxrkxuzr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/ggknptweo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gknsmfkoh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gzoizlcxv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gicptvbto.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/grfbpfzsw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gkfvrfsmp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/geanuitmd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gtzisyilt.sHtML


<!-- 参考信息 -->