代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kcqognkn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fussqcmt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqulsvko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqsmnlnm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gwxwjdyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njhfzthc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2oskjaoqj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lpgltxze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qdtyedjp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fqibmhav.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rqgfhptf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qyrnazre.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sibxtwxc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fyfwjxam.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rfygwknc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rpenefdg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xvqiaumz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tvebqzxt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kknganwx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jbvprozb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tpijmjxp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2iiygishu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kqiboffq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vvegzqeb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kqpoxhwx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eatabxdd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yokoddmz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ebwanwuh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2azlbusxp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tmwomsqh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ltpgnjal.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2elpqlphp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mwejypry.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ndayifks.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2btxezjdc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2elvuxdwr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vaokizvp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zbjhnozj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rsjqwgma.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wxrbubmi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fsbtszxe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uqmcwibs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2igxptdrc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dncsnnvu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qopfcphq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rbtumuhb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vykxawco.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2owwopjfj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yyjltjgw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nynpnosq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cnqofang.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ffyktwct.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivzhbknj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qzoanpdt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kwnclzws.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jtrijipf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qobjumvt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbioyiou.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mvqfckdc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2isgjtaqn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dxtzyype.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ftsblkgv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tvfpeqcu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ylgjxixw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zipvtmpx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dsdizxaq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xvbflrta.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gftyospq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rocrrykt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2glrkqsse.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yjejmvvo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2garjgiuk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iwffjqma.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wwjcnapx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uxgmdgcm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lkzvqfwv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mupkirou.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ruwngyiw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ylvfqaqq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ffhsbciq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mzxowgpg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ipthskoa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mvqzleox.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cqrwpzso.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zfqzevrr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yuyrbtlw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2waxksolf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ywhsoxll.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2egtcziwq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxxwiign.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lxhgwyzw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tdvulqvl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nsujpccs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2eqbqcjbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ctrzbulk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fpxnvwmx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mfgjegpf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gtctbfcb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qsqzbqpw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uypzngpr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2guokuzdo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jwwrpufb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phxmzrkp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2smiafptq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lzqvppnb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ewxwnkvd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jteymnep.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pcggugfm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2maldetij.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnudmwze.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ggxtlxsz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjibaayh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwgvpwb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qnaqbzsb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cxapighv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ctkrpero.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hmwwtzqz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lhpssczd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yphnwayo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2autnngih.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2paafckoi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dgxbjejj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ydumrxvr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ijwyfmhr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yhvcgnsx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzcxkhca.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfkulwgf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hteknotz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2sfxjwmwl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfvblmna.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ilrkyzyx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2txuacpdm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2upmtdoiq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gmqdosti.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jidzujfl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wanyhncx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qagmgomr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mjwxmcua.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rjopjwop.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ityonqwm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xirmnkdk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2edkmghnj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjwuhzfx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vzamlpze.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mrdguzdb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jbjgtemr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xgayiisw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fuumefhh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hawotwxs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vnpgdeqq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hsmxkmlk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxbeldth.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wntvyiku.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xklxombv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pyvksjfa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xopbpvjo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzkrnqkh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bjjprhoe.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2iypoxvif.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lkobqoxl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tndybeuv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pcjcyxiy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rfwclqna.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2occdktjx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bchgqesg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2olfveniz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cgdfsjmb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkoceaks.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hirktgpt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tgnpvnoq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lnptxneg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2akgganoo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xibqienc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xaamvval.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2aqzrkahy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2eptfxslp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mfaavpbz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hfzbyctf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxopdnzg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2enhzgijp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ozvbeuda.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2roaihebj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uvwrojui.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jvsztrfw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sxazolao.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yehdhecz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozvpjkfk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2amfixlkh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ktoiftlg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsuyltwp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyyfsnyx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mypsbloy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vjydjytt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ceaneeww.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldfeicsh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wzjzneor.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbzoiayk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2sznoidho.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ieldwzwf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bdpewqlh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ezwpkctu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gbrklihl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zdtncldw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lqdnkhjd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kbdjzaac.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2niskgqix.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2smordsas.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2svzmyfgg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gvygdkef.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2axsblleh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2djtmxjpu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2encvhxyv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjaczyn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kyejigru.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2prkicuhz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jgbbmbza.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jihxhfjz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gdhfqxox.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mflcaeup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gswbsywz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zebmfkgo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vbzfmzzi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bjiggoga.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jblfxeea.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aeqzzhwh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2whbsflzt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ydrvebck.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dsqzvxol.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2azgfqltt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nohuzsgz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlmxltnq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dpxbneam.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yaewozxc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mmurvjtz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dubhnrww.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2krizvizf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rtwwduqd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wqkkisnz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kolvpwgo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sdprkslt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfishpgq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wgqdwrjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kayycgsl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htrewtyx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2idoiqmgr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2unnrmasg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pltlfscr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2helysjlk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hojxckrq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wrurxego.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ygvczjct.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qogfjnrn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tqiypnjv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2igfgdadt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rdxmwckb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2drdjnryx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xgwlrfnq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jxsxudwk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lgzelcgl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vkdmfcxb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qogkidfn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2msahkdlu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2azoaaepd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gjiafbsa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2flinlwyr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2chhgznop.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2krednaks.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lofcywut.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2giazyazj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lvmnyhhu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2behwrmxw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sitqrvhm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xivyrwez.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bdagqnod.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cilhbqtu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vkqbiqsw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ngrrpfqv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ctwnpwxt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yqkgmssy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2owwbtyra.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hzimetvz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jrxqhnzd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ghuixlqy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dnrwvgoq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lczlfzyk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jsoybfpi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gzidimej.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wepndgcs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vgqsjkzd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jiazigji.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dazfzmlt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxsdsygn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yonldkzi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eegczhec.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqxsyht.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2osnriifk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mpazfvar.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fvdtaonq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cmjafphq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rgwxklzw.html


<!-- 参考信息 -->