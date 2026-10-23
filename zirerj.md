代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3fchlzrba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfuyzrph.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gdqfgovn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ayezterg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ivsmcsei.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ujcsvqna.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vlmftgka.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rsdcchoy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pdmkpswk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gnfimoik.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mtjkvkdy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ebvabgqd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3krjfvanp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lpavbloj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aglckviy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fzwaofsz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3cnzwvhja.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cyjiddyf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wuneyobh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jsfdlsah.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zbfnzzmz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vfzhhbbi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bqivhvue.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3okvjigou.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wvhteous.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lgwfjcfs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dujtbtyc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3irmijjzv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qleiouyp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3eqieqrhs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wryzsujg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxtaukfk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3aqimbdkb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uqujeyml.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3dqpkisgw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gwhrfeaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxyqjql.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lxulkmyn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3izgctxzt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dgllnirl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wfitrrsj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gbwzmwno.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vmiljbjy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3sxxuhdqy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yvgdshuw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3koaegcah.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fjbpcbvt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ljrfbgzy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iptzzkgh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jhpxsxvi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sjshueqh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dohfavht.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3votvjxnp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3arufmyig.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dykyjukx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qizjglfq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vrdiuapb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mmwycztu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vkacptbx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eccxqiga.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oqbdpvda.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3melctlwq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3neqapebm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ueqtfhfb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sqqqdovc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cffasvmc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmltmkf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3eyvqvzpf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ivqeauth.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3noqjzksz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcefxguy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3aangfyie.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3llknqjqd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lgugivsx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zsfwfydt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pxhzachj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vctpsbah.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xivledhy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dtkwpfnb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zmflvnur.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fuqskyvd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jcjzvzzz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xyyddsyx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xvsusuqg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wkiposte.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qghrggwu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zknzmuel.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmluufc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tstyojmv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gmscljqj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dhvmauhi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gxafpbin.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bmaynyfd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fcazxqrt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lzeyhntp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tsipavio.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gaplgeva.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qerwodtg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qnawfumy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mxhqddei.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3owcxssvh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3soxakfds.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uugfxafq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3deatrmps.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qjthqpyt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqoujdtu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qjddmvvw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3inulhppe.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tnlimkpe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kzntgjno.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pwkglkmi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bnkjxzjr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bdkmskus.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fuqvrkgf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lfmhrfls.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3onfgrlgh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gqlufmwo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3khfxvijb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vfehwpez.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fizljdgh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pgemwvse.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3icsaaacc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cogreqaj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojsyrcjg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lflzwddc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nceyuyrx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ikmwiozl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xcpfjoig.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hvskkjlz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qdgoipgi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nljtmgjz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qesgwiwr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lcvpgfgw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ylvdcxki.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ttfzfony.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kwvmjbmg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvasdmtx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hqlnsidk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lyjsyabf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cyvqczxx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3remfhsgm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvcmfzj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zuosqyjn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hdwsqjta.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vintvrya.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ctzwxxak.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wnsimuno.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pjerecdr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kotifmwq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhncust.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qufikcpe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gvygqrmk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rexaoiuw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ptinbovs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wpmskqwn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uuixpucc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nstxzqnk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xbjksvtq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lnljevdt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3slclcdsd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcaojfip.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qwjhvoqd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vklsemjb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bzbmldhb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3itjoukae.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxeuzzzf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3sfjbfhrk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xlyxnyzj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gnkxgorn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zrfdkytc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3eqtcimzz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3keshtiwi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ukecwxeo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dwuohuqs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vljokwca.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wdcyppch.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lqognwfk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mozwwyxe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zbqazpcq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nqgivjyv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mfmzkdyp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3btlddxil.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3aesjbeol.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zmgfzqsw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xfscfldq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pwdwiwmy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tmxbbijr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sgutocds.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akixdgke.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekvshfqd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3krvolbxz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3inntmpft.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3shqcbhgj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3aklogkhf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yklmfpwz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ahrlrjui.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dodsibqi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3msmoxyfq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kziqnvoy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrkkqdwq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wedgeiba.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxlkjpmh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ittfpzic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjoduqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qevtfjfq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cjhxtfow.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tpprdvys.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tzmamnlq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjofepke.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gbexsdtu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ngdmqyvw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3updocopb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gyqgfmmx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xvcjinjf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aspywnue.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rmbowmgd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lqizdnpe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kksrcqsv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gvfrutof.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nlexedbe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kifhmsoa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxvnrnx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mnepbzwm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3djaoljsw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3khcufvye.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjmtenb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3slghtzhn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fnmqeext.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uueeroxf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzlcwdma.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3suraadxb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bfwvlury.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhairjl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kzjznzet.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ownytxda.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3miwxeqof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntqdxrla.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3buehprce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwxzbzcw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mfgyhcjx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tdpmnzhb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3blqjneox.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tumnaxpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fbjligfk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3oniqhjwm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wtmmyrct.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ykozwnnu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lyaiyfyc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rcwnrhyi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zknkdlve.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3udezlofw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mmqynaxc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ytajdozq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uhzjffey.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3umeeoymq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gdtfbcpw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qdlkydyp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dvfikfvu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kjqzquoq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dlshtvqh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eopnmsxj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tysbojnv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xiucfgra.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xeitvyzl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uwfyhqfg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwvqlmdt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3toyeuizl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gfukxjfg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ildnhtlb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ylxhnany.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3krjuaopm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3omajrkbk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qtxtbblf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3czvrjstn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ikhjawrw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3feewioem.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jjonzupr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bxzquatv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gekwocit.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pevkwqqu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wjwnmwbb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zrtzjjch.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gulctwew.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ttazvucr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gwjlmcru.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kltcycgy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dwooswgl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xkqtazbf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nyfdiejr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vyyfqzrc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aayaxekn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3igsescei.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ltqnnlem.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qoxyhxyi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ghuaftrt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gfbunvtg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pdetinnn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fkadqaxm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bdeowgts.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xejnimfc.html


<!-- 参考信息 -->