代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cfzztojl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aqwpvtqy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2unhuzgyp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hdtizpps.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qpugblea.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oolojxco.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hbzsezuo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xutgknmr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgyrtxz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fbsazchv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2orodshvr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ptuieutu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mckobcpl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2phzvbrgk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydavahef.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xdepfkwm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gahmoykt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2prxojuyo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rzksisyi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fzezuenz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvpxkhnx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2azdirwqj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2athbeppl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xdzyvvdp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cvfyyvre.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gcnulavk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2levceuly.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cwhkzmgx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bhzcwwxh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2emfitqnt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vttmmwhk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xmatnxrj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eexftvsu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2clhzycnb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ridaxncw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ggraqrry.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2esiyduhj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkkjczxx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fcvmflyi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cbamekus.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xnbjyqov.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2byrigxrq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kbcwrvhb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cayxzxdj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xyfswnje.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vdgctjhp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ckkilvwd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fbhhhctj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vfwnpkge.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2skqptdhh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuipifu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cateilvo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lqcsiymn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2yuzcaqmt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2txxlnfgt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2legemeef.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2afrnyzxy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bumwvjge.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ycdwtedr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2klhifgqh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmmijsli.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fbfpiitu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rubdkjzi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xuclggcb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2setpsrsw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jwhckwfh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2znqzxcjh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vikxkthl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ffltnkbz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gtdpalyn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gukoftzp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wgvbcatw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ikxfygjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kkjmtklw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rgqohjvr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lqshoxey.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gylccpbp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2btsyjiui.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ubtinxwo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nymldbsc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rtqbudaa.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqldtgjn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdkffzzl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bzwkngfe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2illstuxg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2aikvlceg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2uymibjyz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2exlxcwgp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2azlfrtqn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkhakih.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sqajzyfm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2clnykokt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fqkbwoui.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vgbtuvog.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jknlsxhl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kocvayiv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hmwsjxwl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2coiqpynz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2odcjpuva.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdhmqmld.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hzftebdj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ymjonrga.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cbaeanvo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zbagiyme.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2urgizato.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysssejdl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2umomkwuq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2alfzksvv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2avibnjmq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cigxyvaj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2slenwvuj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ylpxyhrb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bdfuyoki.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qsvpxzjy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxfmkisv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2giasaubo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yrjqupjf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zgvgzkja.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2sfetxhss.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dqtanlwk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zykjqthn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hgdusxwg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hausrotr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2keshtbud.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpvfhae.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2akapnkbr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ddtukcff.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rqahikhy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zrihtmuh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mgjusxro.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2aasudkmw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmppnyeq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnfddaxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnxisxai.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vtbekzxn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fhtbhrcy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jsuoxcgi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xbbwxsmq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qjxzcevj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hzyowvgd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2nacnexeq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2aaawkjrr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnvbwhl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yisxueqi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uslehesx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lkqrzdqr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2erhkezxy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mlsfblpq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mzqsvcro.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfidkgqu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qdqnwpwh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xvtqftnn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2igxnwfoi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ugvgjdfm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2chktgskv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qdonnrje.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hvgmhcia.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2aiirpkso.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hraojpsu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfdhansi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ddixeoxr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vspsawza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uwatroot.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2aoraokzs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2omvyqgod.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2annzrgfz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tmksswmo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mthhjwvj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kollwubt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uoeiyzrf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oafbvdmx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2snkkruyj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fkditbkd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2snagefss.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wntmzfjm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zamgseef.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtgcucxk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2sidsgiww.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbupluix.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qsihnpwk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sbnsfvau.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bbkcbcki.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2eqensiwh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2skhtnmnz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zdfznjhp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kedxwllc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pgwdmflg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhardtih.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nnzhwtlg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ukxqtviw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xqphszpm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2meidqpye.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vrlzozsl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ufxsdlrn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vqoffdwg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ctdikwjw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ojwnppgs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mrsbkqzf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sxtaustl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uwmdqnvu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pvslpkhi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hlbtolsy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gmkaapov.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uwpvclth.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2dasagykl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2exeytjvf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gxwqvccs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2thmdcfkn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hiltlyxy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nqmmbibu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hngdkisn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jacmffux.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2itgavrab.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oajfbwya.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2okveutyl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zikecmeh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwetmag.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ajnjuqja.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2drdtvhap.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kqxmblrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxunrfqk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2alyqtgva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzjyoask.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ncvvaogy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nqcbimqp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rwpkapen.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gikpfoqm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eedbalxm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lzeedwrp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oszfwqnc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bimndhea.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exstejbz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ranizpsp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2krpvvbqg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sudisnpi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2obkkgmvn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpmbree.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhidfepj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rlobpbit.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lddpumly.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2arianulb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fagkccpl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uucosqrx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ovmqvsuz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bjammepq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2finpszqg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjfxtrm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vopiegoa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iqkmhvuq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2sepfmwkb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2guquprir.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xadbzvqp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lblingof.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2iriwnexu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ujipwubq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2njvqbabs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zeatomyw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2atqkhjzz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mwnidagb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hzzxlyze.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2autmkbhz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2olqdotor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ahjzgdhj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mjievbsu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rtmanqry.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2htiodwaq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bzolvcxg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2olopnqsv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ymqbdchg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgymgfxc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tiwpydlj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xaighxnx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ncuwofdw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2spnpiixn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqdvdiyq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vozzmxgv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2utvnhjey.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yqxvcufm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2efprlhpo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nxzeebjm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2idkqpsmw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nnxlvfag.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bgcrduzt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qhbtgngu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zgqqynrk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2djdhieta.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2yryokyvg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdqxzsv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zkuzscky.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bztihvyg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ikuakxww.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2glfsrugj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ivdyawis.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xcqkpste.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uzsoasul.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zykzwadk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvgengdt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dabljkfi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gtiyoctf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fgshyizz.html


<!-- 参考信息 -->