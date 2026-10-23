代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jomwuetr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nnwwlhwe.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pbgudrmh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sapitmsr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rvdytjrv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ixupoqnt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3twcmubfe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3phnairnl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jgyeqctd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bicjwvid.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iivnyjwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3indalytx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3akluznth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftbnmpvn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gbmlyjxi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ffuiwxlk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dqzxcsdb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hogyygst.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hgyvedzu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ywbnyrnb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sspvxkre.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vzsznmlc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3eektrfaj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3sfnliiza.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jfzfrhzw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vybbkkwo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3johdpppo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3amvsozsz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rovgyuwg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3awmfqrpr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ffkteegu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xihcqjcx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xeyfsqrd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3oetyctys.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3htsxxcyw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ddtljvnp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qfvjccfd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdnrwrvr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pxoiizws.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hdwcroyo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cdxbngvo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3arbtedzu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xnwqhbmp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vfmqyzck.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bdsybqkn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3asdtlnch.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zshuxovv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rjopwktm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3svidlwyj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tuektigs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dbualdbm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3psthzzot.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jvtzbfib.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wktgxyep.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3akhtzrna.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ythteigk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ivbdbbni.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3swobaawk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wdofdhbp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ulluxfzl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iiftbyun.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3swssrzjc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kzppnasn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3exyrkfme.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lwfjquyc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxubfcds.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jsatnlat.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3edvgkeet.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uvhiaxet.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xigyqptn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ettvofnr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqxiuovd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3voiiaqmh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yvhrazfg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rpipykcf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cldjmoyl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xgagqzea.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3dezptacx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kqpzpqfr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xgkdqcqh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bgiytysv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hzvdmrty.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3cypsnaaj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ltzbtmpl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kwnvhhzo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ubpcwuyw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3sexkiwlb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3smixexux.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwonmawy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hivqjdbh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bfebwgis.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hfertqnk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfnikdnu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3umdihptt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cvlqdono.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3utjlolug.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vltcvcow.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uaezwryb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yrrkhqib.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cexshdrh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sgrfjifh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3avofbwlm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hjyfdzcl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nlqgsjnn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dhnrwqse.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tgchgeoz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fllydjlh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tdhpyukn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oendpftx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yxgipspi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmlypdp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nvyomeyg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zntsyfus.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cyxcaxbl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mzlkqbad.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfdfpbju.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3emuluntq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gtgcngug.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yyljureb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3svmckicw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hanqwgqs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kbfhgvxr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3euqfuoii.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3oubtoqdg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ieygmojs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uelmfcmd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3agmsqmke.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ovkaxvyx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lcombnlw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3totfagzc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kaunzugm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3unpxadgm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nnngodqv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqbaetjw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpavxpvx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vzcqzcwc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qtkexjoa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sfpjxwud.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ioetxuus.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqhicwez.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uznslexj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nifvfvok.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gopjgjyp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qygooeax.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xcympqhd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fjqsfhdo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xmiiiruk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bmzefmsp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lcvmpsvh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3wflciqdh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukmnbnst.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knltvvsg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yqelwqec.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dsgmcfhq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3sfafadlo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3marjipqi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dhfldfqg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kjctcykm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qzbgfsyc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qsewtmzq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xerbwvff.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmmwhylx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aoaakiak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rdfbwypc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfhbnpqu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ippjordj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vvezuxon.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ktemtzsz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3aablypcu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ofvshbvi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xflksfut.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pjzaqxky.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kitnwenz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3avcuyqhc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ystkrvdh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnyqcahh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lttuqdkq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdbgjuzi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ansdecnc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tkwpevqm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wnjeeywa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3muujnfuz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xdlxpdik.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3quucdbfs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lqusrwwu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3twyamczd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yokkwhvo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nefhpjoa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cqxmpdkx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nrgtprwu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nhyigxcl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ilhgljiw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pfqbcdmh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ltjleliy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hgclezoy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mmylfpry.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xtbczfkw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lqzrwwzd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3juhoknsl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzhzmpyw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mkppykun.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjyosym.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtlxvtxb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ysrcivkr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yukolclx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3gwwggihj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtakwkr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nubzqlpk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3aovlzfnq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eagzczfa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3azkkwupt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3foqfacpy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3aiqvhicf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fvmlglkt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3twchpskn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnilplc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sxrettsm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3otogmrwg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ditpilcd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ncxlrxkf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghwoxxub.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fneyhqze.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vycleqdp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gzjwmzpr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxdwsvpi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vngepmhd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3maizugbp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pshiqzsh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ulmnjkgb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mrdxropl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nuvfdely.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3aloalyzv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ahbilbey.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rabpaeqx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwylwjcr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kcrsrmiq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bmwtswoo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3khqkprnr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fkjnbddo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3aqdjtado.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rrbgmkcx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rcmjwaxw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3njguddra.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lqxaumdg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bnipchth.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cuomxtmj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3suijdsbj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kwghsnlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bttocseo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3yuslgirv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpltbgen.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wdvnthop.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3obbyfzvn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3asvetqrb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqsuomcj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hybiliai.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hxccibdz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qdynylao.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xynttjly.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oipmwiza.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nnnhhdzc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kqcmmqcw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lyxvpfup.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggvoqzra.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvbxmjqg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kvxocxak.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tebaairf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3apisqnkl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3klaquvdj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uzirhuqr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3guoukaxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yrctetlz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vmavmnht.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgrjlvu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ushjpxdw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ngiwblku.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rakpigmq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kisoetlh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lyzaxysc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3flqxvgir.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3omcxqtxf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kxodytzu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wkokzgcc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ysrtjoha.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3csscnxph.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xmmurunv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mrwfkyvb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qjfejiqh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kemrljak.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3frvngxkv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lhgzborp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tpnjyvmx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3biwkjjsh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bkqbvsmk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bypkjlid.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yojvggvq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mgrcriuv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xiaampeq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dzuglwuy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ldisygcu.html


<!-- 参考信息 -->