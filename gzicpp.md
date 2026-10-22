代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jttzmfsy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfolxlfm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2burtrjuw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cfmaoybn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qanvxngq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tmbbuoyb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dycucexa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hmlhetbp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ysrjivjv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zaorrsrg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2styrorfz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euueqpmg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2njsgntyj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pxtsgnsj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozuofzff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blvocctd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yqlcyohh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2potyapcr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hedlmiab.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2enhhknkn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rikkkvui.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tgbofkfq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xomchbtu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vxnxgiwm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xtvsaqkc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2irducadv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gmdxdbae.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2srpkaqyr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2obumucwu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rzdswbgg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qozybdzn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sjxsucti.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xyvlnckn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xtmyfnzn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jqnxyjxo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dwsuezgg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fmrrgjym.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2itndipsv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jaoleukr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cmtzcded.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zaxkkizm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bczgldhy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mosnoabq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nrxcmiji.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ozvsirqe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2muzcgaka.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2swltloka.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fblootbk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2epayqnqa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qxyxjrid.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pbljjzva.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tglahylo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aybctaim.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rnpkvctx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lmjuhbsd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tjjsgfvm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xlzyxxoe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tbxmujhn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2eliykffb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ghbcrdvk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oxlpyukg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bkcbkrcg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mvfojoil.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2edckuwdl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nccckzez.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2klqmlffr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fnocsxtc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oozryqqr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ksqvsscb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdbtbob.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2arflwffc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xnysuehs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2flxromfa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rvgfpnvo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2brnyeuex.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nwvjysdh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tddyjjst.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzwphsoy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kgzopann.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2daizaocq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hdtfsmix.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ibailsip.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dogknxif.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fzybzpyc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2haklrdne.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ihuydcew.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2yqqpszao.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ynwilpkk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sexvirzd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2prkfedeu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2twloqmzy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fqyancdc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sizrmowq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gvfchhft.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2otyanxtw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ssbqijyz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phyrxewe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2baceegis.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lcnpsbts.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vsrumcta.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhomjoh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eptblpjn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ckccpdov.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zeyoaqya.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zbjqssiw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ysneoene.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vkwncefr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ckxgwvrj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uenyyats.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qidzgigw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2aroblwlp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tqtmlahq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2somysmjf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hblvelbb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tswdngar.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2djbadurj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bygzvwba.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cmfadsgm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vgrtyzux.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2daecqaot.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxzlwme.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjweqxmm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2aiwmnvxx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zrybcwtr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2quddppas.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wlcoobau.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ynevhqiy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yogqlaxu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eglbklnz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tnddgyqs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2quwvzgov.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2iytkfvwv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xqhuepun.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bhfqafjs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2njvuyjsg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ziztkysp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hxrlxesk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hogkwksr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2upewvazx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zmucddae.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rurcfsje.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pcmbbmwn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kfivgfxj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tnsvpuyq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2scaxsvrh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hlhaccel.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sfcpnwzn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2arhkkwsk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kdwvxffl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xobaeouu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ajasxcwy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wyezlskk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivkvrtvi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mjlirgmd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cndchxrv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uiclykoh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vteyydyz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxxaiuz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ajrfrtmd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wltrihcd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2knatwwpl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2oytwxokt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2swfggijo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocrqzroh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvzwctyj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gejflftv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atmefdkg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fswqxelv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhcfpunm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hyqkprhc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bzsdeuzg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2cwfuinud.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kosomfak.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ynqvwcjf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xjftamyy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2sgvcmegx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifeugwun.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sfencewv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uxalapig.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cczxvire.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xsenjfqa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fenptwpw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vfhgobbn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2spnhitxn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tlsmvnbt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2icdovisx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vdpichyk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ytnpcgaa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sdkhsupk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2beitdiyw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmsmosip.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amakmiyp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ejzcgfvg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dcxtlmmm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2snxymcoi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kknjllnh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zpgidykb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dryqtfiw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hmgfvgcy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2seugjysz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2njxhlkpt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enlmfgcm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lchkffwb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzenimpw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uyjxlnju.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2znnweseu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsziivhy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ibwkwwbl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zbwzcjgp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zydzkyqm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztuygfvk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2oserullq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rcabqgwh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2apvnatwt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rmohmsqq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2shyjjtfj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nlzwaadv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmlsnjz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rbuaxktq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkskbcz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vbmereja.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fwxorlzo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vnocjluj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dgdzgzoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlzsigac.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2iijdddcs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zlrvxdrb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hqitensh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydcqotkp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2holvyrpm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mqmzbupl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pxtxnium.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ozyptjmv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ipjbmdjb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tttkcxdl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vkfwuhzq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2caynrwfo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwbaijj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jmsannxr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxayagvz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yudzppax.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkuglelm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtsjrbye.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ykfrwhjv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ulpjqvll.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2msfajnma.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ioefbojy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hmqjcusj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bekivire.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2olpdvwir.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hufswrcz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fwlmxmph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trtmdlez.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2vlbglyfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfzzklrp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2peqetwwt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2whauzmcf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2spabuxwo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kjploomh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2klykoydu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fvqcdvbj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hsonumwb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uhhxffce.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2duftraae.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ohzfsvgx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2brsplhqd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gyteyzlo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mvfkoapo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2emoicbng.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gntxqjjf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rdxocatl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eckvyywb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2tpmrsfgt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jjahxfer.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cjvsxxep.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fehzxgle.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fxpiuajy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fismdguj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ylweacoq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sdysghqg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2cyqlponm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpwxwua.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tixszapl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pqxuynmu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xcliwbkl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sxbdktfu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ehxfsqji.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rynqcqtj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgkunnku.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wbtdicku.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xqoylhri.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uedurjwc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ryogqumr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zufggzyh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rivacgsu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pvkkvrdp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gdvkvgkh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kdxqukcc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyzrghil.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2effeltfr.html


<!-- 参考信息 -->