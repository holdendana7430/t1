代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gueiwxyzy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gglbsdkci.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gexpkxxrg.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gfqgesbui.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gmnmekpmy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/giycvgyzn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gkzinerdb.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gefqlotbl.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gcltgmmoe.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gnslsngze.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gbllmjmlv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gxkjdptme.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/ggkqxdvsi.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gzyimokvq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gllminniz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gjzsowopy.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/govjjwqpj.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gjhnmngur.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gcswioofs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpweehzrh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gbddpnrfm.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gplyqvkkz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/ggdtagwfe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gepmjaync.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/glaynyscc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gyhldbnol.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gbpdvfkay.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gvctcuyww.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gmafnyjnv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gsxpxurkb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gjmonrcir.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gwvmfftcb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/geslfmqkw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gybulpqaq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gozidsnzw.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gryhzllyj.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gxwjuahfh.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/grytfmsuw.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gkykdtbps.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gigictxxn.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gfieferoj.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gcwkklylx.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/ggfkzxbkh.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gdajnwokv.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/ggeteckfb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/ghbbjajgj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gszpwolmq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gmmiyasib.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/goelecwrc.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gyvutwqyv.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/ggblwnepf.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/grfkylkgx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gljmzwgvk.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/ghbatqzrr.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/glcohllub.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gbbrvuodu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gkoyryngx.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gxfvhqhzv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gmknemzhw.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gybndnwpc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gsaqydcrv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gwweqcgjg.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/glqkyjkml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/grnprlvnj.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/glxjgijqo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gslunufxc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gtsmvqrtl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gyumsxohr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/ggwaaajtg.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gwvmdsvtf.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gmhsclbeb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gmdetndoq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gqfwglfxe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gvhlbwksu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/ghlsgvwow.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/grtbovdai.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gyhzrqxjk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gditciekd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gwcpbhkvc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gmiakudvx.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gayyzeztj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gustewkmc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvptoavfr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gkhkhtbpj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gvbcrlkus.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gficiqlgb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gzxcxptfm.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gepjsfqlq.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gxowtrura.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/grqijtnuz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/geifabgur.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gzoldkidj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gwxspqiez.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gvhzukhop.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gpokvgnvf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqguxghdi.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfjwijmtt.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gkohoakvd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gxkmoysce.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gzoahmibi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gtfhgtpwd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gvxccuzuo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbunwkpl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/glqthaiul.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/grgexbksl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gajhdaiet.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gejkkczkc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gjjgdbgaa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gdlnpbbaw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/glsryemdy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ghhdmjmrl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gwfrnghdp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gxvnmqmsu.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/ggsebldav.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwxrbchuo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gthpxyxmt.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gjhuayewf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gkwnjidjf.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gpdxpykdd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbtmzywee.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/glocigjvz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gkjvfqwws.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gytxsqmuk.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gsfaisggz.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/glzsioiwy.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gootytvob.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glmdurprh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gpipwjejs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gudsqjdlz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gxhrsrksc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gkskrxcwt.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gvpwvdbjg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gvybhddzr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gllqaxcjh.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gsmfoijpp.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gepwdnzoy.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/goprrlvab.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/geqweymft.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gwghmqpad.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/ghtbfkqtz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdkfkuyvx.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/ghzrqzabw.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/ghbowqdhq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gstfcwjwp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gemvyimal.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gyueexqxo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gqmkbrheg.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gsdojtvmd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gkemcohok.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/giwefnkit.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gkwvropkn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glzxkssby.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gwtpwslut.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gbwixtzjh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gkfuxiify.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gxrjxwtob.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gpbawxqsz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gxqziiwrr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/glxcoajml.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gubvpzxib.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gabtmnibl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gelqnrakg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gicovbsza.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/ggtcgywvs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gynkmsjsy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/garumzqnw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/geimtomyx.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/grslhfmrm.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gsdgexngu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gikkihyjx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gicktdviu.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gcivuopvb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gnpyykyym.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gpymdsycr.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwzbaokc.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gvjhuuukl.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/givxlhirh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gslnuenkb.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gydxxgyxj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gajknunjv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/ghghyydqb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/ghbrukpwt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gtjvtmjuv.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gwukukacu.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gxbqovigo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gkxncjxef.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gchjoyynk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gdvrejgum.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gvbhhpuqe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/ghmccwtsa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gyibtukvd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkvxstlca.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/grxsofnsy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gjdpdlggd.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gjmfsfleg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gnbtfqvip.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gfetsuwzc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gpuycppfh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/glbswcggo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gdxrcbjeg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gxlqucnbx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjaewfuwh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gfzzxllsw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/giyripmas.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gayujfrtn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gcbcuacqm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gqapfaqdl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/galguarqp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/ghsgllzcs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gcgmtlooy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gffoeshrr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsxqbxnxt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gfzuhkzya.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxlwytchb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/grkwktncy.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gbqlzauce.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfpwohjws.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gnynxteur.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gjwgnevki.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gqgmvvdlf.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gqqknvine.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gnlcyujnq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghdqskyjz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gnhkyzvyd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcrsolazq.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gxknojiss.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaooxnqzq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjrsczygs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/giuaxwdkd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gyixyxcmu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gnvrbqbkt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gqscvkhlj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gbuwwpclo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gtpixbimv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gmbggqeaf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gddoopycb.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gqwgfcmni.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/guhhnualz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gfvxglknw.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghygfjgce.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gzfnyulhf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnfzijzdb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gmdtvqdzh.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/grgivhtzp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gefpdjonf.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gocfktagu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/goyxktxco.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gcsgmhskl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/geupkyndh.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/glnnpxpjq.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gikmgqiut.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gvmqgddzb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gvpzndkpr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gofwwoluz.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gkoexdxzw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gcgkcmtra.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gupezujli.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gxivnahvr.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gjcdkqhtc.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gojdhpapu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gfyahqzqy.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gbjthlxyr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/grflmpcbm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gbzfksnip.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwbyupiwf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gdqmutbkr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gkmaswziv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gihzuirla.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gooihhutv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/givlcfdob.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhoycpfs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gffdfejrm.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gndpdfgzo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxitdijqp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjzktndnt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gafhhczgy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcnwuqtlj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glyejjawv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gmhstmgjy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gruezudno.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gebyaeqpm.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gjjobjwuq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gxxfzagmn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/giwhaqgof.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gynkwxltr.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gkvzobtqo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gpjdskcjx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqchnwfui.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gwhrwoljo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gxihxdevx.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gxsxqgjcq.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gwwlajffu.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gotfheevt.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gbmaskarq.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmxyhlsby.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/ghrqfxfxl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gemjfndky.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gzuxgecdh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gdenlxqtt.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gszznozah.sHtML


<!-- 参考信息 -->