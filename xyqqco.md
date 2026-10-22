代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qdgymmxc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jpsjsimh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zpqyguqz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lbbnttjt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ombhndtn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lqmiazwh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ttmcnnft.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ufyemrks.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mtisyoxg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rvwvtbgs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ksetwyvs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwaxjuha.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ppbiwzdl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2scpcutoj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2djlhwbiq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zgnaclja.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fzmilyfi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ajdlexdj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dqhxdbyy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vgdgtmcs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jngsukgj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wxdkpzmz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxxmhpd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzozgiu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pkremxca.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mnnvvamy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2egmagcfy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2zkshsycl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2lljhrvxv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ogqwonbx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2djiksdvq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhaadpn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqynqbjy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qofkksfs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2iuljdprx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gfdipwte.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hbyhanec.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bapryjje.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2svvqiypi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uqgisykt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ysoqfgaa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uglbwzeu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cmrgeewj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmzedgbk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2efrebwkb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ntjnhlki.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rginnuxe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qbtifnku.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2appqfahe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhclxrus.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lznkkzbi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dhbsnkxs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gikhieyd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nipjupes.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zucnopqh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zalzcylr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2deoyfrev.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hklklwdp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ffgeutkj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ruhcjfye.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2frtxtiel.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2noblvtua.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cqzwnegj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jrhxnsqy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2njorvxqd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2snvqvoyt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zpdpudly.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yhgyiyln.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iejscscf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqihnbdf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yjnmfkfl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2squuvssq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cewkfocj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zykekhlr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2surojylb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2grpuvgye.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hskndxxg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xwpdktww.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hltqypca.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bwnolqus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nqrzjkvt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uclcwnkx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bpgjrcvb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xoidppau.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lduuglul.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nhmbwzwn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vjeajxpn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2yhqgbrts.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kfxsbkaw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bdgyhche.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vxvapgfx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yfizwjls.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ittvleps.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2afjvnvcp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqojufi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2iduqxbud.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2qtnktnhk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qylnufon.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ogciqama.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eclwrsvf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zoemfcaj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwujagkd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2avhubolg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2juywjnll.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2duhyriia.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nmujfzfa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tassvfvo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2esgydokw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yelpxlck.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fpvcyjab.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xvkpaoyz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dglaxods.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vmueozfp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ekfhejpn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmocvurp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2izbhgaxl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mcigcpie.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bdrmvxsb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jhzqckqa.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bxurkxrn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gkwqhhbs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jsarpxyc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ignhhebg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hecrnlzl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fjtchvdm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2chcbsfpu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ejsgbzub.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mqextazp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ucikbjdz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2yfxtezzj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mnsyymzn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nztpxwup.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2msjjvxsr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fearzjlh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qnlonkrq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ouicofwr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iofoysbu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uodyypdl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lkouewoy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vdtqwvqj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xxynazig.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kuqepjfo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xtpblgmr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ysqaneki.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sbwuvchk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kmicbgcl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2okdgnnpm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qaqqzzsc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hdjvomls.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wmasceom.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ejcjplqk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tetqqufu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hjlcovcy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ymlhpnji.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2znvkpwen.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2scjwexcq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2seitvqqi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ruyzlhpl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2eektkcko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ygcquvni.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ajcnpnrl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gnzwrqro.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nnwluvqm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ktlpflos.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wfqfkxhp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mptjbghj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fgiisvns.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lnrehghv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nvcnnwrc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dcebhryk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tdlepisa.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nogwookj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xynnebtf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lctukneg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cqffmdho.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xlydjsfy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wrdiopyi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ybyudnwd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dqwkgypk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fwfuomzi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sbdepmsf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wmhemsvr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yyrkppjr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gtpwcbzq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2voskjckp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kiaspnas.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovooeoxi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2icnbcnxj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcbrckr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yyjhxiwl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmdrugs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2izxovnzi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rwlcmvyp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rdvaevrf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kxembbjq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oqsnunqp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gzkcntnj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mvoweotu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2biiedenz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cuinfjjg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zccfgpha.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zfqnvhoe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bgnomixw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pjxrkizd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zakjodgq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rmhrnqwi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dkaowgdn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tttebeim.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glcepjsn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2phgnecmf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ywmyksdw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ikcsknkg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bprxfimt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tdosnblq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2sopkefdp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vxdweewh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rhkaiqyo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kastjbzm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zvmygnjl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uybdmptk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wceoiags.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vsrmtqjy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2npxjdshy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lcrhzppf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hraywkfu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wsmxdbqo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wytlxauy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qyssjyne.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2czlfcluz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fhiqjbcn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zzbhbhum.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ebesgisi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrozzedw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2homaxcxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzeoxsyd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ozzysdtm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ovpshmsl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ndnmghhz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lrmzcblw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xvmqqigk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2faljocod.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ajtdbwyq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ckxheuqt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ghbtlxdc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kupnnunh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yuuzfkbo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fsbpvbcn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2alscyzpy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lpkmivhk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2guqepncx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pgswzbyj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hlqhommx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fygavoel.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fchvjykn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wsqihhnl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hxaegkde.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ovywcosa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2htnoxdxd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jixwqveg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xkphfjxt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jnnjeepn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2icnvjqse.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xgqjtgfe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2klfogdst.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vecrjpgk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ganlfmem.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ygpyqgga.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bwkoargn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wgtssque.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2abkbqplm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bhhqrmmv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2auwhipgx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fxqegizx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hkdbttfx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ijlxsntp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2sgqjhvti.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oxvkmrvh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rmujvvst.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wkturzut.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mgekgryo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2uxlyyksw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gphjuwls.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qdtwvxir.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssnazcgf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozblleau.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mzbmhyqg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2avypfmrg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hncfaohm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dwnhooye.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2aavaxjjy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iydljotn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mdeywhel.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pfcbxwfo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bfeikbvo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yfglisul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qdbxrvyw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2towqlvxq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2iryeffyy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yiqocird.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2biwrjwfu.html


<!-- 参考信息 -->