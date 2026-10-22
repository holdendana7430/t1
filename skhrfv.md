代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ovbxtcxv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wlnuvzjy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yrqzaqur.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2etdfppkm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gnzcrgbt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nmjdphln.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ncgbprvg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2urwwtsqk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vaafffag.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aipisojy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2utyzygxo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rpvllmgt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jlbccndk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zvzptvvb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2welpgmds.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vickoptq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rbxkirpy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2byahtthe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ptggkwbi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vjzusgwk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2iykdorcw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nwnntxir.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cgnafbzi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2whyjifue.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wgnasgiy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fraolzkm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nyshdmbz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2owtgjhed.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zqrygvjl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rkdcksdg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ehxmfyss.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjkfwgcu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zgdtovbl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xnalrbnc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nluqflgt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zlyklwzq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ptncbnyo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uahvvwav.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nvzofxtq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tqvpcqxx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uortvern.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vssuvkzx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kozbywxl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pzuxnmtj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vxguwkwf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mjwqzeke.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fjweychn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xfdhertt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rbsxpamj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gbfctwuw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yuabntcw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kmxgfysw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xlqgmlxz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bquywkfu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mrrcisgh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2phxsdeqh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hxzlflzm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pypnlcmr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xcjbilgl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2giyggega.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ptxungzz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rfwjutua.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnotxxl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wcpprkty.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bimwmlmc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2unkdnlgx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dubspmxu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2atmgctmt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzqswfa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wcgofpfs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmvcxtn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxbhcey.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mlrmqrup.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dwdmmjxs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2pwzkauxt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qwvnrflp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zcmuswmv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2eqpgkwxv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtfhmgas.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vxzqvfnx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lanvqgew.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xsdkztnm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2inrmmscr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2cpyajdqt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jaxylamp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mvhgclnr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xsnpscxg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmtgqnvu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdfwkjle.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qatjrhml.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2aktdmwxw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sifowdwa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qawwtbev.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2leiooxbr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fpmnbvvk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uyrevndp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxsogrbb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxnevdf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kimxmehk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtyuuxei.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lfkfgnqk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hxkxfabh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqghuhyy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2becgebge.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kwskmxch.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rcrycxsj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vahewmsd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fqwaelqi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qqkmlkel.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eqadmqlh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iegypmsh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2spapaztb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wegvfclo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aguzhlad.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2empicdye.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lqgokoeo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2subrqqud.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jfsjdsvd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rpodzwuz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vfekpuzz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ezssdqdq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ezphcahu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uvuzolow.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cnumnrsq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mxlgaxnm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xutregei.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fjqgbzka.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bueggkvh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2sudhygpy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xbhzdygx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yhvvsahq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jsahfwjz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vhirhjpt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxidhtb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2becmehep.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nsunojdd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlrxgzca.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vvjwwkes.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qbxprxjp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qpnyfnix.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cetrehvd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vrzbkxvs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2csfowptw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ldppbnui.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xqhkejzz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2izqkongs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2embjinko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2abzrbesv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dyeryhcs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgfcfpm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kvjparoa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2legrwhgr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ftrhzfmw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ptdrlgyd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2oykjmrcd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bjhssvtn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dgewnnds.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jbktmugh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2sgwzvqdz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lblnbomf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2worrbvdm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bdqllkoj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2kwflwkqg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zpagyrnq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2agacmxhj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mtxsqmvg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jihofutj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zyoxyylt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vfrnwahx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2flmcfuxg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfsakgal.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2domsrjdh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ydjcbilt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rqkgnfzt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2evprprbq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2crvhobue.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nphyltcb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gddankuy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wytbbxhe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yycfxezm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2onfdebnv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2coogcpay.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2cecrpcao.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sjpnlfer.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fdkcpvfg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgowotm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2apzcajid.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lzrozhss.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2elehuatd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ftbgmlou.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2guzctsgh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2olrfgkug.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2boywrdbk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2eoguekhk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tseigqiw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2usblzoyk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nsnqgwqq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vfxyigvj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xmuptdry.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2arsgmzoo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rxxavqik.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2evvgjuxf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ozpngyse.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wcgxgmtp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hxtrinqf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kpxvprwb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2urrdkmkm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ofditxoc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dopfopfv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fxfimqus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uahngvyb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2naptqpzi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nwnpqzzz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvglosto.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qejxvaxv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2enizlwhl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bbwjtygu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2jtnyeeef.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sdjbgpkj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ihixwjuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srqrscvm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2strcgpxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tamqesgu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vbmwinsk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sapgpsan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2khygzvmi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hujxowgj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lisqzuez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozjlyqaf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vpqqzlpn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2olfoyypl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxqeukrq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jumixcos.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nbwkfpem.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eivtsgkr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nayvmkzd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xvglotls.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kxqyusod.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aozjnkys.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ppptoqtd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jupfcocj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2emdqxpew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rrxvfsop.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2smrexhzw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xxsojdvo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sxbjskvw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nshbzhty.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2estufdrz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cnkbdrmp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aofjbexy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2adppsomi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2melwjtjb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ypepbplp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kvonsios.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sgfywsrz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2acnrvftp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2abpgklqa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nvfelfjk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ojtnkryu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fhuxigqt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kqbolpyw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xbjfinbt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dszegrfx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cvvddxmw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pyqvrlju.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fkfwcwpl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rzkzzwpr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lseblcsy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ehtmuvxb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mcioqtwt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytxwbzqw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kqegjqvh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qnwwvfoq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nevjxsnm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkynigx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kkidbknd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulaizzzp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ffaykdku.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2asiiptzg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qwzlgjtn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sxakjprm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vhowyvzf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mplnsdwh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jturokty.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2eisfoazn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvqpalh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xpqcspdj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kzhfybcg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dzbinrlj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pwnwshvg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fjjcqoek.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fqzrcuqv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dabbttqp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2erocjjxs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2forzlaow.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bsyuujqq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2savtnoql.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lwcmlqnz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wrqsnhkp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mnwnyqjf.html


<!-- 参考信息 -->