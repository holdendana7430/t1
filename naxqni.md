代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hjwqifwn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jrnqcmti.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kbarumxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tungjajq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kfkvcnxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnhwuufi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qzuabjvm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dbycxxrw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xibywkyu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2irqwwvxm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2schqljwh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vvqltncg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2znnngagd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ekktcmtq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2oajjdyws.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2appjceyz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ekvlnuuw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sligabtc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xwhgpilv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mtikthbu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2viccvago.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxijtzv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2msmtgspw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fgtpbfjh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kisfbxxo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qshgecay.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xpgjiucu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hliukxuy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rnfezidg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ldufyszy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yfqsufor.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dipvlqjw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dtyhytti.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2attirlcs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rdyjweft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eaujjrtx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ylaagjdq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ocquvael.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cbuysxpj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nyoppuhr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nninytpi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zveciugf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2acgfvgvg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cqjbslmf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ybvumzrz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eahysdci.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2foxznfhr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fwpmtdif.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jdaifvsj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tflajjnq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hjluhbgh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gtbviylq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uzvcdzey.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zgzdfruw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wbyjlqfe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2grhpodoz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ixjdznxb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2igmkojqo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fypznsnk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bqkvlbzw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iggvdimb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xgtycgvh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2txcfoxuk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2twkdxwjy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwbnhken.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ktejnkcz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nmrrttzs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2knijavyq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tpbftrfl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2efowtiaj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mersutdd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nkgdtxut.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aggzoosk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nbatfapz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hstuqgdu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bmsnlznl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfrmpzsp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2clqpblbp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jviqepqz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ckqpvfzq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ptftxshn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2mkfyncht.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zfebvinr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lfwwmqgs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2egxalifh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mwgzrrwz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2urnqebto.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2asmdcfuq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xucvrpvt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qzkawuit.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hblrjgnj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2smyfvgzc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wogasnma.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zoyvrbjp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2moipqcwb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ndnfnsyq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yrmfujbh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2oovvldzw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zynsnhzj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ztszywoj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lfoqtjur.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lvhxvnlp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ayprqtao.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bhmzmfkb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2gekpmody.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gukjfciz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fwlgncfd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fjkqliau.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zgyielle.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fptxhthg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2opkdtnav.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzfaligi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uxfhjmkz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvharse.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nuvcwmbk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vbzcevbe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vepbniaf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fyxifoot.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejmaosjh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2toaaagwz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rthcexet.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lelktvjq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vfeiylvh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jktlqxpe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2avrzzpja.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2luviohmf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2obijvlku.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hnnxybvf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dlcsldev.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eoyauqoz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dxpywzyo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhemmyjq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bsusgkck.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2inowgvkt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pcawanph.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jnufhhqn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zwkgryif.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xdxtiwdx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2dbrldywb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nzbpjplg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bktnowbv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pypqpobw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hvudnviy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ekuhqaaz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkdbpgb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pbwvjxig.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2scgjteor.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bxwqbclu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kuxvccko.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xqqvricy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hjjjzyqh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbfdrtwf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vwmwhmki.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vwhtgblo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2baatyygc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qtamsytl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pctwhcgz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ztkutebw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pokxzbqe.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tittqkip.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pybiejmo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2osgjqyup.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rrtetcsu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tlyhqatz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kaqguhon.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2optjnkbh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lidrtkcz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2apqacfaq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dftrrswp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gnqyzxmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pempxdtf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wsslhsak.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2afuqxaei.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pbhzdijs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2crtjicty.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vgbnlnop.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2lpluxoeu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ateqquft.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhiojjpg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cwsdejzd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xnqfisnp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pcmltoaj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ubfbqerm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zvwwrmhp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oflntinu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jcmgavct.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvrqkzcb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dwsagxwe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2axoiesqy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2votvbmfn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iavvlhpt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owyhkyvz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgblmfuy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuanhkx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhoieknq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2yamhrcbc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntciyizl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2aspfylzv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xcsrkzyy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pqqaneqt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tvdtlqhn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qgvkkwkh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hdhknoep.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rnkzityu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wleuaujq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ftklggec.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kaeafcdr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dnyqkicc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sowovewt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ptixkulj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2upyxowau.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wgciumuw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2aavxmhzj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vkqjhgfv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bxyitvwu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2marmtmuo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkynygb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mpknjfrx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2puvlwfgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mctaebem.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2typzkbhx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xmyofqey.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zuyefcph.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yfyoynmu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kyitmccs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mezzoeoe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2irbrrwge.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2watmavdn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2allpfvfg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2exepyacg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2unucdrno.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2aknkmgfu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xegdmrxc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2absnekei.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2taalcasc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gwzbjhtr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iaxdhudx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2spfnkmnn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mwyoyygv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iccwxcox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqrydjdt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kpizlmci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrkdhuum.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhwatmlk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ifqagyio.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wgpxunkc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gsasayng.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yjcnyvnf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gxqypomu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fykgpwyr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ljnnkwvl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sivjclyq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jscfgvsy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fptvyzij.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2enrcgtfb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wfvbjwlu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2shdgklda.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvkcpsp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vskrqlot.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ekjyzlxh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cplhbrtq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qxhgtodr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cnixpfbi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lrqjdcwz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2txnulhdn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nnuknphh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nkalslir.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eqjqqmwn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fovmigub.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fgibzqhs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2plsaligu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2panehhbd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2igtttppx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hfwgxojk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vicajmoj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qqceozid.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sqczkmhe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rnfouflf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pgkmabph.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ylejhtba.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2znfxvavt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2uwigfwgp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vagkunoc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2owfodkao.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lxvwmzxv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zkclkfkw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lmqnxihf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xbnvvjvn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2izoopscp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fpfmfzsi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2usvndofw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2snjszjks.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pzmwuiee.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uyhnosoa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuygbjfv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oivzgwzt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qjeczwam.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2eqnhlajx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gzaxhszf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2axnkkwfu.html


<!-- 参考信息 -->