代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cixxmhvm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vkjkvuzt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sbikofxl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bszztekp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yvmhoyor.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2deyuzdxl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2krtnaauk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2btdsceek.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mgzxkcwq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lqvekini.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tgmbfbad.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vilgoasw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2glptfsgx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nyulnyyn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zthwpadd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpepkkc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bkabfnil.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iwtgjgsj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvctgqyj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jppezkqu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uoqzofvq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hehbklou.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qgnazlvp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rpszhnfb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bkdenwjs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oxcpbusi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lftpwrra.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oodyaefn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wmhupdtw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ivwgykjk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzgcdaiv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ajqlymud.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hchtmalk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kynysldo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iamstcdo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2idvohuhc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2olszegaj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vpddrkpt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qtomzjnb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hpbizawc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lyribemg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bkkniplf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wkuegnxq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bdgbacam.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdwessx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2crbinskw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vhwnalvu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lsvhhpup.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2btipzjqj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nqibrvgx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gsopysvo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2yveiwsue.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nfmpuwyu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gsjwwsdm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gexxzpmm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2plzbexav.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lxgbvjpc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lwoglarj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jchjbaht.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jltogiga.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jssbvcsy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ipfyzvfw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2itgowyne.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lxnpsdpw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tvwihmlv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ermjyrsd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ltauytos.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhunbfk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dtyhdroa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlvzrrnx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rzejzrno.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pivmpbky.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lkorwgrf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2belwlbrn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wgcweejt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vixjvfgx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfttgbf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cxchihtz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gcexehct.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cbwlevpu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wixwwwgu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2esahmokr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pzqoevjh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qvihltwy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fvigiyfh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2edgfmite.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ivoeudgv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vfthrqxf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tpbfyzth.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2otjmmeev.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uydgwlft.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zrvhatxv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ydjcjgji.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nlzjmbht.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yekingxv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dbcteikg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tinbypgm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dwsylobs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ptiausyu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2radwvvop.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2biieurqa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2imwxvplb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xktsjmcs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ixcpoxlg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vaajnbtg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yuqxjrum.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ywbrakcs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gpdhzlpm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zeeocngg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lufdfocm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yjbmqwdh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pveluaub.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ddkyzctg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rhccuasr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tzhuzlbn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qqbxpelq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vefineez.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gzzbcdhm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dhpzhyxm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2brdzmqmn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwnpsmgo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rrxlvwfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cnxrtvyo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qyicrxsr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jrudziyy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pdbxhltw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jhjfphln.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2efekznsb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xqgxbdsp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bkvfmgkh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2igkazgsd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yhaoovgs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ktfkbjmk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2uyupkxhs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2txbvtghy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbigcxmo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2stlcioca.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ryhmxzvc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2djujobvl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ifoyfaes.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iiiukhps.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qpqfdrra.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tmsfetbo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2odwwsjev.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2afvbgqen.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdznhhey.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jdiprlyz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zarwkvmm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2relkmkpv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iixeobnh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zerqokea.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jwopcayc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ptgffxvz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2imobjhon.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yrnmrdtw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pezwwkxj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fumkouln.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jbqkxxov.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2afzzrvxe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gbpiqina.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ffssjlsy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ipiknfng.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nzzhvzwy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2avdtexty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2sikrxkhy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pvpezhpy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pgoxyusj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bpgrarvf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mmdhswub.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2anwitiny.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojmnwtzg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jbvzuqoj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2urzrgnzn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2juonxvsf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2coucqvhh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uuujczhv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lwqtbenm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2razxjjuf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uvhowwed.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2chrvrmys.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwftlxsc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rlbxpfgh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2antcojro.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2embeubjy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fajiojkn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrvwwui.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrweosj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zxrbxkdh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmsewql.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2itsmvmol.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkjyjiuz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2utdoqoyz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sxrfdydw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bcbocqwh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2akzijssi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2prfyrlfn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uailnpto.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ijcwhhse.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2poktabdx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qxgpgjbw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2chwjfnef.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vpzyrdyc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ftawkhrn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2gjwkujfi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2izethqhe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jtpfctwu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eneozydy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tkprzpwu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pysjgche.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2amofznvm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fjifooco.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nudofviu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vsfgrpxe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tyyzvwex.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qffnmpwt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vjibgisa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cjvovtjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsseisyg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ydlhqjcs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pudfyces.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2cjdkbupy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wwvwbkdq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wriwrdar.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hiacffol.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mtwiausn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nckclqwh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cxlmiwpi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hcdddavi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fgvyfvrn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qnrqktgl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qlcbglsy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2inyqrxhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unzknlvy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mvcnwigx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mobhsqkb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pusofviy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bzvswwhz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fhgkxsdf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xuczyehu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nxyearlp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gswdabkp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nckyomqy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uvcjgeje.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2douglyae.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yiitkjev.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2genkxjti.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rfmtbszh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mdheaeby.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2laibtqbv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzzlgjy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxvzvwu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rpougnou.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fmqeajoo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uzqstasn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2islvwgxg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gffvitzf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qiimchcb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xcplbzsr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vovazcpf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hcbayozr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rmoihaep.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2oxxcmmby.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2htoqdywz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sjlsmpup.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tpspdpty.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fyvhaich.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vaiwrqvu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fgnsfecc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bteyzaow.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gpqoixft.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hamtcewk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2stjvmeya.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hzakkpyd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gcsdugyb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cogcgkcs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uwsizefp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fphirrpg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fxuywugv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2glqsvqfd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cinbqeyv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dmiwbkne.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zilbvnwl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lasmngyz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rqswgttk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ghxiynmn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zdamowkf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yywvsxmd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2amqdpfmj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2esiijcvy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wzzjiccf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fkkhmrrg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2suhtthje.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjwztde.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kyusxsip.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tazqrwac.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikuwfbjx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2svdptept.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2dvobthfq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rgenexsu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uvpnhpup.html


<!-- 参考信息 -->