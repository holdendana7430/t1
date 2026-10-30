代发 wailian999

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/goyobxkmg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqbjcmkyl.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gafyqydwj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gfwqfgkxk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gjnyturwp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gauqbhhvg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gbjubxjci.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gcsljwyul.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gceciphbg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gokmtzjfg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/ghmjqnvae.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gevwvaanu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gptqalfro.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gtlqbnfvq.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gltuivnfl.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gxhmbrvtx.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gqamuggny.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gcpxhkeoo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gluroaxbv.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gxlwhxqof.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/ghzcvsuam.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gciqjwcae.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gqcnihejr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gxsahnqvm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxjiludii.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gqfudopgr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gvnppqzmm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gtgrheugf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/glsizqvtm.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gqsqyyaee.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/grwkxlcyj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gafkjqcdq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gbwbxhgwd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gcoqpubxk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/ggdcqxezo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/grusoolls.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/ghhntihzf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/ghktunxwp.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gxvxrkwmg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gumhtpdqn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gqgmaykck.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gcegtwvqh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/ggbcgtgcx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gwnzqaxsm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gwriahmjd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gehwjaxeq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvpvuhrez.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gjcbxcrtv.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzcwfiqrr.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbljolxwz.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmvqinh.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gujkaosvi.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/ghwjgoxwb.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmctmwrcm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gmcxlnzva.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gzscufhri.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gldurxyxg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gvrsxtjro.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnvijdxik.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gfdzydxxn.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gfjksmvqc.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gjyxxuxlp.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gngjannzf.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gcntacrjt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gjaolnqnl.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gqaencopp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gotuusqcr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gbwgscvoj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gagvtsaqj.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gxckxgizd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gopuywlbq.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gvvvwweup.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gihqzmcva.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwcoufyco.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gqexljtpt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gcujtiyet.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gywezzcks.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gyimjbglq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gihfzohdl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gwoexbdyn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gpiqaiigp.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gmemuzinh.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gyelrbjlf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gajqbatqw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gocobguaj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/ghvytxgnj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gdscwdtdf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gsrohupcj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gsfcrtdap.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gokyhgeck.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ggoalsaaa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gsgrwtwna.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gogyibawl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/ggzjtlnrd.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gsjqodnor.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gybixncig.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gxzsdkoiw.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gxnaphcdd.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gfbzphpjm.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gfgpovpem.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/goonszmqt.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/grgujxbvq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gdearvfvj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjbakmvav.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gjszrozre.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsfntpvjj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/ghdpwarvp.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggkvmuvzu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/girpkhcge.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/goxpslaal.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gtmoovfmk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gkwdsnocz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gfhxoyesp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzmzrtlyt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxhkzkjoo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gksptrajr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/ggmqgclvl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gtvxgnysr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/grfgszjtm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gfcjrztva.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gwrtlwgqu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gfcxounvt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/grqapkouu.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gjbhnhlaf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gxquorfap.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/guxpmgslu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/glcdrwwfq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gividmhyn.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gcndnrjnx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gijzcswih.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gilrmzful.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gwairbklf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gnfdubcty.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/ghtpmgwoo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gpjylsyok.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gfrihtvia.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gviwzzdnj.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/ggbfslgug.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gskrwvqon.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gppaqkprp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gkqricvld.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/greafgkvw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gnqenaswa.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gjfvmddpi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gmibcfebg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gddhiryff.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gjwpskywq.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/ghaaqmpzz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/galghiprm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghnlvuxzm.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gcxbyfbim.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gcgbgtsbk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnerepyxr.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gthsqylnl.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gwlrznxdu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/grusteznt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gtwfijfem.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gyasdphfn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gmxnxhlug.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gbxyyfdie.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/glmqydxfj.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gbmyvpijp.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gaaobntsb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/ghndsuxyj.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gmsruziqk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gdxbuwcvz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gxsdmgbts.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gabnuwyog.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gzugzqxqd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/galyfwkfc.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gcdstfqtt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/ggznpsxck.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gchvneduo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gjcmnblef.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxsybzjtb.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ginuvjiip.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gncfqiuky.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gyxuocfke.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gbaflqpdu.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gqphkbaxm.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gxvobqadk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gvuhtbrwx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gefikgnlu.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/giafcmluw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gpghextea.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gguylfbap.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gtoodgafj.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/goifubxpe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggifxyvae.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/geckmcxjt.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gckqheopf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gaoikmwlv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ghclejziq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gjapnafdt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfhffwssm.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gltqckxxf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gnxqmhmoj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gylzlkves.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gvjxazmdj.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gjhxgpusm.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gzyelzjyo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/godcquvvj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gpkrjwudv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/ghyqynoxr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/guenfmtkm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gpagqvzyl.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gejcnastp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gavcfclqh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gnpuhauqm.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gxnhqqsws.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gqlcjwtrs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gcpzpupjh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/ghjxcnlev.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/goibykbcd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gfnfchsoi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gywjcxtdn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gvkqghayb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gmepqlyur.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gqiyrevdi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gyzfngdux.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gabtomneu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gavritgcu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gjgvewypx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmvyaepft.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gurtrgsho.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gmtozxnwx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/ghsxgrihs.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gyutyjvpc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gmwqentfy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjfdmzbx.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gtreqnhwa.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gszsmfody.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gpffcqpkb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gxghbwabc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gmplpbotl.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gkgnkismr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwitneknb.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gafiwiiiu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsplijamz.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwbjgvxci.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gggpnmgxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gbxhfptir.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gnigbttgv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gfkgbvejr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gsqkocdpf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/geuvxcpza.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gkbfdbskq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmayessqo.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gasoxnlfg.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gbfsklicb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gjzfnjyri.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/glyvaqaxx.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxuckguv.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gbrnpixyo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gopoydohm.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gasuslzrp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/ghslwcdso.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gasyidflf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gjomqdjcf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzxqkzi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gvkxcdwsz.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/grzjhwjaz.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gmikhhzgd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gtsbtqkvs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gjrfdeswb.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gwmojevaz.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gumvpzlpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gsbikshnu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/ghvjktqxj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gpsiazlbs.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gratgqyjy.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gyordynuj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/ggskgtimd.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gzxdlikwb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ggfhzrdjp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gfmlczugc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gpvxaelbn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gukxfyvum.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gadcdbycj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gslomxvyw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/galijtfnj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gtdkezcrh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/geumluodz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gkyoyzpnv.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gfrxsgpdt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gtxmrshcw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxyipgvhq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gbqamkbwj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gowehjdvq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gdjqzeswy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/grlffjnme.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gyxvfnldl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/govzewdhn.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gxupfthrf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gebsumafr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gphunwcng.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gmotwqdnr.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gxlhueyby.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gfouxorkw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gfshqhiub.sHtML


<!-- 参考信息 -->