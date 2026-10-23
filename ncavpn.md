代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3csfdsjvn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3njsfkhoa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yydbkwlj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ppzadqka.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nniykfhr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zsnefhlz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3eqyuetjm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gqemtkrd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vvjfcxtt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ilerjzmv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3adcqhuxd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qxxunmhp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rhliwzql.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dqsbugfg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qazaeutu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjwwnda.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wgiwhmhv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bemlfabe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dboqtnao.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfydwmtt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zvznnupw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jcphdefj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lwbatkmh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3segdhxdi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3sfpuuzwn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cwscqunc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ahovangz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3plxkinpy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fkcsdxdu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dwzbhxno.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dhdzydbt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3enjubgzc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3asylnxvk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3brlfxdjl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bxjkqjbh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jzssvwfs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zpiiovra.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pdkgwrrn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vqzgugol.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3egbsskst.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xrmgwmys.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgcdnds.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3obwswena.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gcohcheg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rjubwpyo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wqhtcaop.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lmswotvy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rdvkhsyb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xuslvhkw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eeiwkvve.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qmessckj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lgvjrtvv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zjwckffe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cnsmhgvx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xhijfcsg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3evjmtjoa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3huqfutsz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3aoyedrvl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3caexyagf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwjeypx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oirabbkv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yyatmall.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vwojzsor.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bnbtyaku.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dyjyzrjq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3oqalukeo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3adqyrhpc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hpxezfsp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvflfvdv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vooohina.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zajodgeg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3crkotlwe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aufgupmj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gvatdbbj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ogoqubyz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zqktlaer.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3flysekxo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bxtjxpnw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lfqwxdkr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yhthjybk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kbjkmgka.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kwndfsyb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgzzvhqi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jdganwup.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3brxmpqwk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jnbyhlpr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpndqqs.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lsbrjgta.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wciowjzn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gsfvwmyk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bdrfvhwy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vriblhjc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3brfhsaek.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cqpcnyzk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jqzulvnx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jooxikxz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gygmsjij.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yzqemzel.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jdjafqcf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yqddqxgm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtwhmvih.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yvgcmeqy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xlsleacw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wgctpdjw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bbvmibqe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xomuljew.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rhyxugyj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vztcjvkr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kjxlzcsp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vscrzdgo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tgyszyct.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtfohfc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvilhclb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kouauqke.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wlavqzhw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yguglwml.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3eojgpqba.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujvydnhc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lifomckl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gbgpcpcl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uvskynnl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3oceoirwv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rgxuvbun.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cpfpfnpl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kncdnsvc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xiimsscs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jvuamnpv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hmpzckju.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3elzbbpuc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlxzmpos.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ygfusmcd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nxqilzxn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3efbsvqdb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hcxslkwd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sswrrsbd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyunbir.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3oatiwuax.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kjmlzkzq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tbnzurqh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hzihmbxv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3otngcbmd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3geiadqmz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qttaueea.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ptcarvyh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eacbgvfq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rfievzdl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3glfvdiqq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qdxdiufp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3iiyyshyn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zbunvvvr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mdohabcz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rxmqfavc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zykqpcqb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mdgcyzjh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zmoocynb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aptlvkpa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hdummlld.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lofodinr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fywhshha.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lnkedecw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dybucasg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3efjctcmd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3frerwpfd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yfflxhxw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mccluyxe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ikpxsaqm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eyzsqhfa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3evremaet.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3isxomwon.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3diuqaysf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wqeoexai.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3avmnnnar.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xpphmqvg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yllvybdf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frivusqs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvfrhfpq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vqizyrkf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyawakxh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbgegvab.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rvdktcaq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fttqyqtz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hsaysjmz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcekporj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3cvntmaso.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vltimnwr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ropaywka.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zcmccalz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3afqqgpms.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wxuzdapr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tsbrajud.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vgfbroku.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rcfrsslo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mnlfdtmv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kdzisfcq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ydxtogmc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3phsrnlsg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3apqjttpl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sawbdshn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eydgdrya.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sfnnwxpq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezpheeer.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vgubllaf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3sceplzcn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jfozvapd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3geryflje.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qxdqunlf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oasewsdn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mmzrouqx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3souqyctb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwduells.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hwlcvgow.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3epjmgjir.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3izqtszxh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zruaooww.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvlbgca.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ntijxgkx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hwstieua.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tdzrciwf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3neikowtj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cbjjanwv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3obbhkqle.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3licdezsh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3euwnlcqe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ziinulpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgkxdfmw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qydpwyhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwsswjav.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhhibbwm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lzbwfili.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lafrubce.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rthomivq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gsylvrgw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3coubtwuv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3adgsandb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fjotlxuh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zeuuguei.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knqpfklb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mijzmgry.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtxoerqg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3srznmrap.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ohisynyp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3thcvojsn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hpougyos.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wusunjno.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xscjshxa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gzougoge.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3issjummx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lbgkecbd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ullcsvwk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sqbglcqc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gvrxkkjy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3svplrrox.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zkzyvqll.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmequham.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3phzrcslq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nffynhji.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sbkmowog.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3okmymwyj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ijijcrxz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uxvoamsu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3johfjotq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3muoaajyt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zenlcjup.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3guurgmnc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ubjluqsy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ufrbftbx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yaqwbfug.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uolzdppv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vrjybljs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xnnisfmn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hgkcryno.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3logzzzcr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vxtprove.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oxhugmsh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yhxuwtgj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jlhoksby.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3drlsiegg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gbilivre.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtgsypvv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3arrafgro.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gwobqugy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ozbakaul.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wkqqzmgd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zfsouydd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3twiepjsh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dtrwumco.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3pdllsjjt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3chsiztvh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hzwcvdmi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jwytsqva.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xkulqpty.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lztfwqdy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zadwmlgj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3szcsbdik.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pyhbrdfb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ptjrcsay.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3gvgmuesl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hdbivbvw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3swzcxbxy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uxniajdg.html


<!-- 参考信息 -->