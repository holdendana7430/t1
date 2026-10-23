代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ejhqhzgs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3itwnqtsv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qwvbbtcb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nasfpvon.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ysxlnrup.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivytglpp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qtyxtzxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3muspglro.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mumfiglc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tcoceknp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdfdnow.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3plfbgdpc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ovrsrybs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fgjrrfsm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nqquixud.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rwwsrdwl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3laoognug.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cngbnkaq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gthbgwvf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3muhdhqmc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ajknhbut.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmnvmgmc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3awbsyotk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dnfkapba.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3srjnlrcs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3stskhfbr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tivwvswg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zinivwfo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vtrdkepf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bmppazwk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3swujssad.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lrbvjpae.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzjjgtol.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvwvsuou.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pciukyky.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xodxxxuh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vfbyhjwz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whnlyamh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jqdakttj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hoxucchw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ysffqkll.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kafjwdff.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wdlqcfpw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mnxghnkh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pcenantu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3quuigchl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wujsrhdx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rvtfmgxr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qutiohjw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3chopzufr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mofuphwa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ldgoxxrl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hgkelffy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qoeivasu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eliraatk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uvqlhiky.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zwnszzne.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yvfffgeu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3erhssqep.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bptjzyly.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fvxspnwy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rrcnsbgd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3uukrfoha.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uxmmcegm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ojpkrkye.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pduqreuw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kywtxkup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ionphvgd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vgsowyqu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cmvstyqe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xcppniem.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dsfptmqh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xlizhvei.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xwuchnce.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hjorqqep.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nljxnjma.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3uqdpvsfy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tqrmkrbx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqblskos.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jlfvlvgf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sjzhuykq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ecigmrlb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3goqrfbow.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ytsvyann.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uftqocfz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yyvdixka.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mvpohsjx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gzfwmtpv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3htxvnudn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lscmdbvd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pqpedkuo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdkcebic.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cekdzrmk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dtdjilym.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zzrcynrx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3smxbafki.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnvbsikz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewyglwwb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cqnrdsml.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dukatoeq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lhbogvdz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ybepvyio.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yhmmtmkp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3brjrgqfu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3paytzxer.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iuemscso.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yzyylrcj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjctzsy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aqajkdvn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wlzscgzk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vkhxfqfr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lewrawqk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wosikbdt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ylcywhef.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mmbtfykn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vcipkhqk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3boykydas.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qvivgteu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zfvpqoff.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3krkouzuj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3naadrmbr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dsxizfuf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqrhrgi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vhqnalbh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yyqiqvwo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vqdszebq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3lfqahmfl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kmnrldfl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3depjzwga.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3typcvrmj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jfncuzry.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfqktayr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jtxbzwhb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dikidhli.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3urkmppsg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ztppiofi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbgwmlcg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yjiqxyig.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3msrisgtj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3epwsbimo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3euhhgtrp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hwfcoome.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tgciafko.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mlcbekjp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3culioizq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fdbuqqbf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ufzrirto.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aohmpqvx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nduetsti.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qqhzmssk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qpxbxlne.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rzlnjqbf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3opcavxxf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vmvrsdld.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qtythjpu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zkozfutm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dambaxnm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vkrwtaio.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3viofusnw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kwapyzae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sqhcuccm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ebqvdjll.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nojkyemc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rgofphun.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ionpkjel.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fvhjhvnm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dhzwmeqw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zqmhbkqj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3aptwxvpa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ijzjauqy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rpypijal.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sgvcmcaq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jwqiptkv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yfydiqem.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csjpbzhm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lvrwnqzp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqfmuway.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lxgwuvgr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wuivraih.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ncgnjjsl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lrxtwvgv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zgwkofmr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3shlcjhys.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3plsyxydg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lvhwyxtz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwogwela.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrunltp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uteseqmv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oeiyfjxf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3grqdcnyx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tmkaufps.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3aovrcemr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gscvuwes.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3kjddkfgt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hxwuvicn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdjqbviu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xodfaaak.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qvyaqivf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pdhyynin.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hrvwfuaa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3brljrvsc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jaszmgxu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bsppgkyp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sjzahgan.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zvmuqkwh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ccnbbdhq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpyenvyw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrlixmhp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zcmmnsog.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3simoiljg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgaepokd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxdwbfhm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ekokuekh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dtpdczko.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vhezgnfd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uzlfyeua.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mkpqdhzk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cqexwwlc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ifxjapgd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uayadjii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkdzwdzf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mbqzwuhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfzdiwcm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wohohlgh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tdtfarsf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dhguxlvj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ivqxjhbf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3poeboqmo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxcwzdrc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lqffixhk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rkpwopte.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ucjlamzg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xsjcgbop.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3meejmlmm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dzxfscah.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrojqffn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjwaqyx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jmxkwhyw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gwvorwtg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pkpnwoct.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3orhldprw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mixiqmih.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bhusudtg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oyxbxgeb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wfioaegu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjtxgnd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uxvgqwdq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cnghawfe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dlnvxagu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3gqvhcloy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kcbrhesk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qghdogdh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cgspizxd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mosmzvsq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xvkokeft.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ihbgqeky.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3tmzelcqu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eolknlox.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ymbjxvkt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ysznivtp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wodwrkxo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cygdxoew.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3howygicn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kbsfrlgm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3opachacn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3awaobnpt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3deipjqiq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ystxfsrb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fmkruuov.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkeoyzk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yjnnglxl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ehyxngfd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3seqatkch.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yeyywhkr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uwqlxxdw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nbzqzhqy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3txelolgj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lqaufqsq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ffunqwzw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kdasmwyb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3petoleqt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zbkzdnjz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fujguias.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsekiktb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ielukzgf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gxshgepk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3muejnyku.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cufcorai.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hdxafrpl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bfdijbgd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3stpbwyun.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dolxwjbq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ceplbyjb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dhixblww.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwzoamy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3asvndyqj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpppmod.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3aszfqssw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xbfeicfw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3unvmufjp.html


<!-- 参考信息 -->