代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tklocygz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiqdlbdf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wjqtospn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ykvpfmkg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2syitteuw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ctteugwr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2vjyvcptp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lqrfcojq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bzpcfzpc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bfpsvizu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zeisijlm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpdlabca.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zxrtuvcw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nzbsmfgv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2giiopsue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkwolnpg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hdkybynz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjjjhome.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ezsshtat.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zlzbsoev.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lqaospqq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jovpcmdp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pwibghwh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2yrtglaiu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kjohfgrp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jypfaktk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pucfkerw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hogfaznu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rxckfvha.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ehpajrox.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dlsqruwc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2izhhgyrq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fnahcbud.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bhbfsflq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xxrdpnob.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mogkmpws.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2eqkrlqck.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hdufbbhg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wvuymtzj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ppamoodo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvqfgrj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gnsorbno.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2miggubsb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2knranuxt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hjcjxfpq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzeifoye.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxufayk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfllrwmn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cnidhzzd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2njmnvrvz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qdyvmjqw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2njyvonnx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zuiwrvuv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ceewyjle.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ernbtcqu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rpqwxjjc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qzstaetu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sfevzqmv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2thhhejvs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ejmgkgml.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ickvcdht.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tlczquhi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gqaublfu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nrdhwdbk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2clpbuwsz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cjykoocc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gxcpdcnl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qwkbbtcv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zicxwdmv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ekddrjdr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mkpnythv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2znlbcyha.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2sqhttxko.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2iajloric.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yuszunyz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhuznjea.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oaiiwvgg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jpruzswh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nxrhzgcw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mxixhdfd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ukgyvcqz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2akqbgcqq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2okvtkokk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lioecbtp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2befmzsoz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2summempj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pgoknnof.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pexrcmju.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2beljfdpe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ajsrxegp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2davgywal.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lawkijxa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xlqsllot.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pcjyogcj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ryzhbjxg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ixbtiocm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdbvxijl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2abdkfbvu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zpdrnefo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ramoyxxm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xpkhqkyq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ochfxhfd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mmnytyvg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rxpjjnor.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aqievqem.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vbtkpzot.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbaaigf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kpamriho.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2uqapbvxb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kdkiuvwt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fereihbf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uypraayf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hfbkzycl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eyrbmlnd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aeulwswc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dfdwpnon.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qzvjewcu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2oawlnxnc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ndtksonx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kibtqjzu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fsodynty.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ntuxrxbk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ayllytek.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqxqurcd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jncfzykx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bpygwmxg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wjmkudne.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hvxbuvyj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nswakotb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wwirzkuw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2onfvlwwg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kejhmxaf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wcauvkxr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2deuexyol.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dshpspxs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wplarqhg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rhqaezsj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zswbuddf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnranxxi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnloqbwh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mqblcpru.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2soedfwjs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dcljtemq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2foeqrnyf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2npqrezqs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hreuqthw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kdcsibky.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lwybzboj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qompvlkn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rbvbrwva.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kzgcgjsf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qtpekyro.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gfrhbhxm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vcmqczac.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlwfeiqh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pgbuxjuh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uczzindk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvggimi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vihwgkhv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2igzqyhoa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2izghfyyl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hswfmmmn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tnqsdgyx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxqrtfa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uuaufwbh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iflogmis.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dodoyssp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2yhqkhseo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wfoplppm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2weeezepk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2grpyfsth.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ijunhrra.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xsmdynfc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vtaigcti.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yownrort.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2leheumyb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2pxpeoovi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bywumrwy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bpomrkcj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2psiwfsav.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wtfsuknc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdbqddsb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cxmbxuvv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sxnqgjrl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2scyxxgqf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2plrnnuno.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gqyifxhg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pqfdfysd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yihhriqu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fvjevgjc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqasvwd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pcwfpybo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dxjnkpou.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kxxcsuzd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2edvjgyjl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2egyaixna.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2adnztnhl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gudvjixp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zuuxacsy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wrvpwxxk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jywxngxs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2paxxgjfs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vfjlckbr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yepxozsr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2czqorvli.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2krgwnffg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gbqvamyt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hdqlvdxe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqowylc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hujbadjc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gikqnttf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rijstyba.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ztzsqgoq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tvjqyqny.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qtujjlqz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2swwgzrtp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2atidkzkj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upingaep.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vbrevwsc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2neyjejtb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrwaxuy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xcubmvgg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2itulofjz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nadydddy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgxqcbi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kiufxtps.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zlgkcbfn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vawxornd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iivrbrai.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qtyvpkmd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ovpqlvqu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hqukylsn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ezltyzta.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ynnrubwv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2msknhook.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pxqxztmh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vmueawda.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2myetxunh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oqefjhyv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pdtvzjxf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nzdoosbf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ynynkssc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjdvfggs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sovkolxq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xapxybyk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uiqenjyr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bptpwxxz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hbcuxcny.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qtrvuouz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cefdfsfi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ljtrpljz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxetdga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewyviupn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2oeucjldt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyfprgsc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pgfywuvn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2thynxsed.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2txuxvinb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wtvmorxp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ndkdladp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dukzsvzj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bfeoziod.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wjitnufi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wawotkxt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lslvofbo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nxcoayic.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bngsygbo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hvfsajet.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tixjgslv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hxsggerw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvjjjel.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2udeprfgo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yqbyauja.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fasgqtia.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2suqvgjpi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dlrqwail.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rcqdxdjz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bcoqdekf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2akpxpype.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tgnvbkxw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ogmopwal.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ztdynhkz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2djbporcx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eedxkgyq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xvbhrsoa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wvqhfeud.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ffbimnnf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2suopvdmi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lcvckgfk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bmniogiv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vfkewavm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2giddgkfc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fmnvxsow.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hvtgqhjr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yivlegpd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2elciohph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2szpdhmjs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2whveopla.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fklgenci.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgasaej.html


<!-- 参考信息 -->