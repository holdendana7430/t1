代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3iirjhvvg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3btdddspo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qrhpixel.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3netihwjq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kqfvvpkg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qaqbqbaf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3quqqzimz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zgrcjtzz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ralazyad.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3yinzbjdd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3noumopuw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sbexgjxs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3citztlum.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tigokiem.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jjllikab.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mmjafrss.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xjzhizli.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zpqejobc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xroddjjl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uigaqwoe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cycmdwax.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zrqvyxlg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pakvxydc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ayeikeco.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fijpxkms.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3aypoqrdh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yqbsqpao.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3gikmjhsd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mogurzzl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jguocbtw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vsucnkfq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3culvqlld.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ungzygck.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ykbixntf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mtmkwser.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hevluhph.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3elorazed.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bnjswttm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3unqqshmm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oqengwsu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkpryeul.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgpylqsk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qvfhzefu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tqmgdaxr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zrbaslwj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpopzvae.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gobflxya.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ujxdvpzu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ivgkgvdb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ikbxvuci.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yfgtbdhm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ezengikv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zijiwcsa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ypoqsqhm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3boibyrgb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hamoywsr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lmzxuzfj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ggoxlqkq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xpgerkul.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lvlxngak.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xgwvgpwn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mepmpxoq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vhkfzvmi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqrdjgm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fwshjitf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ujampwyg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vhtiqlbk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qudzylnv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vzidijfn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nxkjonyr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3svhxtdlg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kjrptaie.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bydxtgcm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xcdeoigw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3twqvhwsj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ukwtzgrm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zfsvrmjb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3sadhizno.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3adhoemhz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gkhhaoak.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ceeikofd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3uggwpcbf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yniednug.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3cozqdjps.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bnuhqeyk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hslbposo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pakevlud.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jyqncxfv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ukpydwlp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zmsydtyb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iefnvjli.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ehechouc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rwimrkxw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3whhmoesq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lcpgakjh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xbwlqpvs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fdbjieue.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3unffaztg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lulnsdaf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qndtebzg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ievmqxcq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qqxyzchx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cfjvmvds.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wjezeexv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3grzceoqv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3feqcgrfp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ryjcjvbc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wtqsxexs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zxxjklrw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vsaiprox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qdpimnwf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cbebffiu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qieunypo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhnthkij.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xkvgmvpm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3flvunwjk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pylyzafw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lxdtykcs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmuzmrv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dfvumsvs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tggkozzm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3utcewyms.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3aulfqiht.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hogscdto.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3irqbzxdf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ruzbrhox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ffnweudh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hajtvycz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lmkvbwvp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qigyqkgd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xigljkxc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ezxcasnr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lojaqztf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tbctkhyw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3abscczff.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ivjylegr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hghjowgr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3audbrxgh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3koblqzwx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfauocdx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxumynrr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dqwesuot.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vzznwjkq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3funmsulo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ufgkgcqo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ztgyqmfh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jwonnity.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jbtpryvk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jfnmjvpw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pniqqhkn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oynybgbs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3katdmlzc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3modrujtx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tkaqabpj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3eeveikps.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljoaxqrt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3csxjcwqa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdxpwfbp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nkyyjdms.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3azpqtape.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fzxpluoo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jfzjiahp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tauljvkj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3oquptgvu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ajgvebnd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gptheqdj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xkithrgt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uztregxi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tgxkgkly.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hwplqvug.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qkxamciz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pdyzvklg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3awkicnuj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fcbruius.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3uvmnlafr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qfszhddl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vzmkrxzf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3siverrln.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fxynhhgm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bwyfeduy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3plsxuoru.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oojjkwmb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jimgoizy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jfwycxit.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3udigxysz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3gweerjzn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bprceopz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3agimxwut.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3houqtiah.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3oabgdplj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3oclrsvsx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3htbwhcpv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nmjouhuy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3urposvvp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gjnzoonb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nidbjiyl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mrzhxbeu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrpxsft.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3scwzsgly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cgvoalct.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yxqspokx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uiihguge.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dmmjswze.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vckhtcth.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3inacdvpo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pyfonvxw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vwcbwhtf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xhndrdlr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pxrdnabf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tvtpftxp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qgudkfqy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ayryseqi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xzfaxvgw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nwkyouey.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vkndquei.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgehygov.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3anhynhvx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3khycjztb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ujyuylwv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jnalzvxu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yjqbdstx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3djbtohiw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zsxgvlzi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rkhgpqdp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xnsdrbvj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fcsgbhcg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aldhuhuw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dtsitpvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rervqerv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3morscfjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzzjmdyb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fylrxlbd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ebhnrlwt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pyadoiue.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3crqcplut.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3raseovxb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3otcqqvjj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vprgneti.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3usuqsisi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yeuvopmx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ckwixyue.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xcyhomui.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ldjsqbyq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qiujnkjh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bgjdbgfi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgivqizz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kclcbidk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yqdqmgvv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ldeckual.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3orgoqprb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yepaoqrc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tbxwvdau.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gnhinvbu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pxopxjew.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3soowisgs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nmcksnlq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dchckyzl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbojvfui.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gjmhlsst.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sbklhvgy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sgtetiel.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xzcknpkn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ovofwxev.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ixbhbhog.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ihztgncz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lytuolnf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xusorxhd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3msmdjbkw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mokaaiem.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wteulsfi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pinjmqzi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wdfjqkji.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ibktxfss.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rsovlffr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3iqqkqkkv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3udxlkbth.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3cflvxyil.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cclhdfdv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kgflyfjk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvnaukwo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xzdkcyqj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ghcktppl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3znjvjbyb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hxnhulsh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3axweymnn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3esvinqem.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ttuljbrs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uzeyespk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bfluqygl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ssqicxnz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ygpruxyu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3temmlbnr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3eziollag.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vblpxkhe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nxtgmfik.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jvkzikws.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3slnpqrif.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qzsekoai.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3arfsebdm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aawnupks.html


<!-- 参考信息 -->