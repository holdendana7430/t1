代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ngkrouae.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gnfvrema.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lxhdggsn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ixptggxd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2cuksrgbh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nlbqqnzx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mfithgfk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2alpkcjjp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pmytjuin.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2imribjjd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zvusfjnn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2txxnmsxf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oqpipltu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ygahwwge.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2odjsbvbx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yycgmrlp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gtxlmiqm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nuggjqpw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2brakslvy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nnbvnqgt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ltqpeojn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xrfaammq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2izyokeae.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xhzgtldz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ataoddbz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2igbsrfhs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vybnrwpp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sjdadfld.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ipvscbtz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2sunzktgf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qjibdoxd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wehhhvlt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wxapzewi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mkqpipjv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rxngngyl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yzrgfcvp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zjzbvvyq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lmgcxaqh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2joyeuifs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2djpzclpp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bgznbwck.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2plxpnfbh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2omxslhvo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dqdvhsfq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2elxugjas.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rqivtdjb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ppqzziyh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kuxksyqo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fjkocesn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2annroozp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qepvbdgb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nqrxwuig.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rjgsuztb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xesmrhly.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dbphfcpb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tpaugfxv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oqanmwkn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2sahygvsp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hosaqxdj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2caxjbbeh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dpiprrfw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dubhtgzw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fglvlieb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2sltkzrcg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tgqsemyz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ynykzviq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zqmyiens.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ajditieq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtoaaops.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yleydqlk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jiefdbeg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wdfuswde.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qurkmghx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dyvqfotn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zwaijent.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ofcarpfi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xmeilxqm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzdkbgdh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2syttqxbd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jknfyvig.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zhynhayw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mlmpbxvd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2msshievu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2taepiknp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2crxqnaaz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hikschwa.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xgyoetyz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2irjyvnep.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lkybfwxk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xvopzilh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xmwcvrcf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vmjjolzh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nzqkkndi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ofuaaiiy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zrvyftrk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufnhpkrm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmewsyk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sddjwcze.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lxdvvdef.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqtblhau.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nnddhhku.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2iynpowaa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ocupkbvl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jpaiosbs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zmhnxlki.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ymwubviz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ixmhmhlu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2skmrpcbc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wjewppaj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wefyphpy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2btkdrvpk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2oxdhicxq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cigtkplz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qczfadqv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2doeosleo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nbynesus.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nixcggox.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hpeemqja.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ihqihkub.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ggwuubek.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ahytoqts.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ylbzfamz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cbynhqtg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pkifbfrp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bnwtnwpd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mjnhdrvd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ppgqlyyh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cjvvsdnd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qdvvtjgw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qyjxkeru.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jqdhqesv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqikwypx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kpqymswd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2syzfkkzh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bvpixlrb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kqjuyjal.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zocppjwe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fdkgbsfk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oirwinpc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2widksjwc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ctphuqaw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2esmludzv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fylzoanu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ohbravhv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwckmdd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cdogkuws.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tkmlmvqa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zmjgnhhu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ewdkzmqv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fdavsfag.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ozsmslis.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hmfiriao.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zikucrxa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jxyfxhbe.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cftqsrgg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vfddbayw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jxwcpdhg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2snwoqpcm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vbhhybdx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2aqcadtfs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kcykpzgq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zpcspuxb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ksbeakvy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ijbgqqsa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2owekmwvy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wdiojkyf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdooodp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jqrwgvvy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ajnaonmd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dkvsncmb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vqqsramv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2obwzdqer.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mpgijzuz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vkjshhpa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jiovvjwr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lxltxzju.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ezgqpvng.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2poxlodeq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2weuabadm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wwlhjcmk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nuvtqfyg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwafhovc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fmxphivc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jwgbniqw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2voaticux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tzvnudvy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxwafecj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fwnxdpds.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kinbukuj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwcytdn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hfjwehev.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kjesgdcy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xdzadzgc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvpuxux.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kknyhpxf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ycysrser.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vdcqaxzd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2czqgsadr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xyfyekhy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ewzlhkgd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cdbkfgmw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ezasnwxz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zlhwryab.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pizbngza.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2teqhfngn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ijatrkac.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wgzpyfaj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2dvdtlghr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fsmifvvy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2umjzxgiw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mcdnskmh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qpqnmfnq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uwhrtrry.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fakrdusz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhzjhld.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgmhhwpp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2epzstkhd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzmgdvcv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unbhlitb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vnbygzbd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cxyxxvxh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cwwathzw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2deielowx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2exwhbvft.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lhpsnnqk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ncinoese.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qapbcmyw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2poxflgrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thldpnvn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2swnypwzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjcjbpcw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hrxsytkk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2luojxcwj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zncvyeih.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yqiwzgqj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yakdlqbz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2enxtnlnw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2evhdugct.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vbgdsdrz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2moqoujpk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2glrjpjvu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cugeqbql.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qiityvoc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aviiieco.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrawqcik.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fxxflscu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bpxfogvb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2picvhygm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ykjvyqly.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vmeeuvjv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2znuymcnz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gbbezrrx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jauxqqcv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rfjzglrw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnpcazn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xjshrnzz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2reilasjm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bmudsmai.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2prjnkakt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2idgaigdc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ffllzpfh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sduggawf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aapwqmgb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2htmnvodb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qnhvreiy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gtfefgeh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dgrpqmgw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uwgssxkg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hjsyqrdc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yqmagdym.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mrjtkzrx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gqdsyjdw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dosvmyqr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2epqcfazp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ojnjlils.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bbsknfbw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2nrtngpct.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fagkjlpj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ogrknuci.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2odtgbewv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2saefqkfc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtqjldu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2babelick.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xctttunj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xynqpfjx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ksggdgkn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lpbgkjiz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ojerrhsh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nswaikgp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xbbsbtdk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wgbcervt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvuvgat.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tvctlsvy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zwqpdeoq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ybnzqlnu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2adpkbfdd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2llezehbz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhnnjltk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oiwgahmn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrgfhbr.html


<!-- 参考信息 -->