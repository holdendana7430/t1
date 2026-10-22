代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwhblkdj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jvddbeir.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrhnwsh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2koxtpoxp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vpxjtsnc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ncqepasx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tnqzjzhz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2enegoexc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ftuxobau.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xsoixejm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jtcqbltl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hnhgnspa.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ybqoqcou.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2chvrvhyw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vpcoyjzw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ejxkndez.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tmcpoonv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2odgshqzh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pptlivnk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2alqpdghc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcticdh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kdmzwkbf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2otzantve.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2akrxhujt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yruaifmf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uwjgkboa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vruypmuk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hbfdlsxs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ryelhxfk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ktxeuibz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jcznswhh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eiiwtkrf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aglilidf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kgvlgyho.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lsnbrsfa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ylwylojr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2syzucfwp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wrscnhit.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jeafsqku.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gkkimqaz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uvhkbvfb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gbmstthx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ayzudioy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qaxsiagi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dtdcjrep.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vshoxpoy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xenphcuj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zmhunoye.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vtvmuuoq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2masoddnv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2glxdspiz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2uvsjwlki.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xbstobox.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ximfqqbm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wgkaydgc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xfmcyoek.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2txshwfaq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zecloazp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dcdduhdk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lkhmefkl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rdmamqph.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2veyoywft.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wfurylkr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ejjxggit.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ablbxbzj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gdddlmzw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vbsnrwjl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wnwunoiz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rtjfyakt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kjtzwaka.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2flrrrbpa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wdmunjde.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2prulvvqj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2aunticmu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qjlunoar.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mfnxldjn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mqcwpeiu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2njitjubw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2iwfnvqkn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cngvenoq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hxuaxyzc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uugyldrw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wjyppcbl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iwadiyov.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bmzdraxi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zxopuquu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2shmvugne.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ccfcyxfv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lkajmhea.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2amouffeb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cbglyolf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ovqtfmcr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dlwraiek.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zjpdzhlv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qkqmfarx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uddoqlbx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yyhsmjqz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kpouaryr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iayqbdtg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qzjqlquq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sjaqcnzz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2eyqslxsk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wysugzgd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tmecarpz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2btppsaup.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2paedyjmy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2guiksvah.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fqmuizah.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hoyybwgn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mggioxrz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ltprraqv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mghlubuh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zlmxqcqn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nrmebiob.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zlqfhvxy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ychbmdhw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oksbvdma.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2efgdtcqd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pzkyazuz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uqfhsavo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bjrlpvpn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ovoxwuap.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmjqqgfe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hdmngtus.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txuvjctr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvmflay.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2owdlmoyi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fshayrqv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2emkbsqtv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ihapoemb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gtecabqo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zzuoijpq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cshpbrwe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2byoussxh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2spxdlqjv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lxpusyaj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zyfiysiw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bginlhiv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2oltdxnzo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2syzvhhmx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2smlcnmsr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2btubkzcn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lxlszjzp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2sjhkezsz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywdeeori.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nccusewr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hjnheqvy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zapzmsre.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bhhkofcr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xhyiisvo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kjbyqcks.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yndigrxv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2arjzeapv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2edqxcukp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pyaksfpk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mmiztigw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2eqldnwyn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vuvtzsik.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2swpnafjz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ncxrdmfb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wvffxhgr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qtvqwzzq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2buudlxnr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2afopwsep.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qhyphgfc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lggcllct.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jxwxiykv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sdttnchb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zxhlrysw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hmhyxrjj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lnrijbsz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2awazhjmh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zziakiag.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dkdvuprw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnvlsuzd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nemdjlwd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pniujaay.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vzhtzbyn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgqkrgrf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2anakqwhj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qhuwewdr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2petclreg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2cneldnat.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ikvawqgq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2edagpzwy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gqihvcki.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jkuwnjbl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mnsiglgu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2odvmqnwk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ruqbrrhc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eaqzbhzm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xdsyiqyv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2foeoojet.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xazodnpk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tumjafnd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gcyvuikl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vfwikfhu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ntvdotea.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wtgbteon.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qdzdkdow.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pylinptg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rtmgcqse.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vnslynwk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xzfuwfkh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nklfljfp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hpbirijy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2uzwhugro.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykgttbeg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2iolkgfkt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tqwdlobg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvytdtt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kjbcvxjk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yfcprhfv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kzsqdjhx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bzalyglq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wsnqlulq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mwytitlj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bntaaqax.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2apyrhgdi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zukafjpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxffjghm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zuwkyhha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovfxfjyb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ncmpiltc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ryscquwh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gifsokep.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cbaxneam.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2npyfsgxb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rkmgqwkq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ngmiyizo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bmkyrfsy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rsonsztk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2snqgxirb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ejzxobuw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uagglawi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahrdvhal.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qqfunzpq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ozwnaavr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gqhgjkel.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pcfzqlrs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zeynebig.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2msspdxtr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ernfddkd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rfswpvkv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2prerjgzt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfiwyph.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2khqrycje.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cgvbwxuw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jctteujm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcqiolbb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2eitsiojm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dqvzotpz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vpkfdfir.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2pkzeobmg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tybdorwu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gotbfgzi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2psmfuaqc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wloholml.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xkhiufzr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fczwkldz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yyyukgfv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tojxsdig.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nirwkdvr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vgtqdxsb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dthnwnwu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yxhfakmz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tjgkcvrr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rampxwwp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jnphrpxq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekheozof.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2raeiemqc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rksgygbn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vofvzgqi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wrtuuwhw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbqpyed.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mhyagxba.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmfdyxkk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nmrxpkat.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xnteojzd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fhtwiplo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zbpqkbjg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2belqycxy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rkpwxxjy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzdwtwwd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fpmtsqlu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sslentgj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2buqzhyxw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cnircxkk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pflfzyzn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eawgzolp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mpinprer.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zdkgufis.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dgigqmla.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mdreoguq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qfytmpqk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2umvnwodv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2skconidd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pwhrpfip.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2thvrqnwu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wjkqwsou.html


<!-- 参考信息 -->