代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dkiljkez.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xenkvwsx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wymvnsnc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnhgpakq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2syxzjrka.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lwyizuwe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gnmsgzjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcrkucfu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bhnwnokj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mobbrcfz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ujftqzlb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hlnpxsux.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lifzqjeo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hsxqpkpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fiklhrvu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2uarubatk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2unpnfraw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jbewkvnm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tsyuwijc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ubhbdaxw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2brvfxkco.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zyfsshyi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mwrvwjjr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrzjzkxk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gplxcepw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2imgwfprd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2odtfizpq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2czakgkot.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fmqpqbev.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gwfrqdjk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qwqoyezn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kdbothto.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jxalcvef.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qdsxtcal.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2erbauwcy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qbavfmfv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kojmrzan.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lxqxeyii.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2waadlafi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tevhnytt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rgtexnue.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hbjtwdvq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sdcpjvmq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hflyhiqu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xuwwpfrv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fjvfamaz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vpzydaul.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fjzbmcgf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jtzeeben.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vlnpfkst.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2flgmymeg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ikoqzrsd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oyxwyaox.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pzwbbgsd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fvxyndmd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vaffozbs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkqovvsw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tpdkauad.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nsakbpyk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mqclsalj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ymexfolj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tzxgbpmp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cdekovlz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tktrqzdk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wjtwqbjd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2stvoqxkd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fzgdharz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nlsoutmh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2isacetvk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oxckgyrk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ujljuefo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2iilydxuw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2frvjhcci.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wgluprwe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2kfssznbk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ydhfibxu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ywensgjx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2pukdvwvc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnarsrdo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zezarykf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yanocxtd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vagamxdh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cinorbdk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vebmbuch.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtsespui.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yyxpmdhc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fjjeumoo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2iooshzyk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mysfawww.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2snrtsvny.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mbqmcrxm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fchpuidv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jlztcnyp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wvwqkmal.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hhhgqsrh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2heyszfch.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2poxfhuvz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hfaaduoo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xkywsjgs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pdmzyewh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vgjfeyvp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wvqkkvol.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2slkuihnc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nfkrnlxv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fkkvogtu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oxlwbeqw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfkepvir.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2geytekcx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zhraodqu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cofttsge.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2frbxbyal.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvrxylum.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qemjcjni.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iczusubn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xbtkvxmj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2myndczmu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xvqbctby.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wshvmtws.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cxlfgqnk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qgwqbdfi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jilssgsq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdjcnxkp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxopzkzx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2enxezaxw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2twzturiq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nruucznd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wqnpujya.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ujytpmyd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pinxwnqs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oujtbtph.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gyomikbq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzrtlhhc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ikshgkeu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lfbxvuhc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozwozcpo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqkwfkhd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fweyofah.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kvuhjajx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vtcmzjdm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kzkealeu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kefqmjfg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gfcikjpf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wdsbeujh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jknsswyq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2snzujjyu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xeqluxfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gphxzzno.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dyauisdy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pidhadzp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2snjpgtfs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hdvvpivu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gxfbgapq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gwctqrqe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2gwbzgrip.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2obzpmdzd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2udluihag.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjfsxwfo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcfxlxuk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qcquzziw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dtlbsshp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgydbcw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wfajwzid.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mzodtwip.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tiijeksa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ijbsrqkf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2shmboxwc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kiedamff.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2eydujttc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckhicdoi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2svneobop.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pxshraoh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2utjshjsa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2falhwhuo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2oidveyrp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bqagkpby.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zsrsmoni.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfvnhhg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lbvglqpr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iwmcgcli.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ifyjpgbr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2phvcxmzd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gidleeaj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbpooqsp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2laaqutec.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2utukubcc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pqgwrwoq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nawsgimb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2oyxylqxq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rnxmttpm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ykmojavm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2laupixlv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bwlqmzeg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2iyjbnrap.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2roniveye.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hedctavq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2moqdvrvq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2huoetgpm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2arbaxqer.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2odwudqgh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rlcqbtpw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tviwgazy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2nsunfgxt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xhvcijfw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2znfexarj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xpeddnmg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbslcxh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ckiwxaqy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mbfjtlrk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2emcqkjja.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fncqkhus.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pyuokshe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhusxwx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yztzlgrk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2beoqnutw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mvkdredn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ndpwnkkp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pxaohata.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ywtppfxg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wemfnnwy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tvqwayog.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eutyqkke.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2emoeknoz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fgvpskjs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qfivwwen.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xwbvcvdk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bwowrtgd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2sckinlev.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2coknrzhv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hbuyxtag.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zltxqalx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2gzzjfpnw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wthtwsxm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gzrwuyav.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfeswyim.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bxpylraj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tzotdwpn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ihndiwnu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzoajjzd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yswqwgbt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rphbedii.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pqllnebt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mobpsjsx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jfqjtctb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2venktsiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2feihwtsl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mnlfmdnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2debgkuvl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2erolxhkk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uozjdexw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2paaehgiz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ttwszaer.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zraazwjn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jkcsrmhp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gqetsknd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2smmwnhub.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eimcfruz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2drpkfzwl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lotoeahe.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycbjzxnk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rzxvshzy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2aifisnol.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bidxbuhe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xmjtenyq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ntklrxme.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2twdnciuh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wnqvybaq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wyjwwbyo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vbivcgbq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lzhcwhxn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2teflmrxd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wetlmsci.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fzgkqeko.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zonmgrjo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dumrszmi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ohqfbglh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uugoiphu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vwmajahz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgeqtwp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hesffiwt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lnbvianz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2usyirqoy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2newjxnap.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hawnykfs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2tffeiaev.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2debibrle.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yyidijts.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2auhcealb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xhlkfppl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lalteynq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uzvbqpgc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ipehzsfq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtnkhcf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qjetbwlk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmvchlzs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rraskchy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2djsvconw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rwicvxjh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kgznxhrf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzoounzk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jalkwonw.html


<!-- 参考信息 -->