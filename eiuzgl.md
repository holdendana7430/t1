代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ztketdzf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kxicnihk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rebggwuy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qlrnpvoi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3stwlacoi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wcqlezvx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zwblcvfa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkwurgdd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hvjsxtwe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3supeeeau.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtitbsnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxnvteex.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3eidtoqno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojsgmpad.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ffachdgf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wydmhqms.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3umrojkfc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yqcjrfzi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kcovcahh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jwpdbjhk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wypdbbob.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vbruaqmz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ikxahanc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zzarhrsh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bevlxmfo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vgjpjxnl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsuhcot.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eineldby.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ssxsprad.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3epqrltws.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cflidaxr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tvburgys.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kgbddgyb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ysrgvwiv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qrhpmqdp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dsmghbul.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gikaxlyn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eultauvs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qngulvko.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zdagwhtu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gnbrbfks.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmugzqcu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3owqpcdet.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3omkhmqsu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gmiarccb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghrilgvw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vzxzczkz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wukrqxxe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgoksyuv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nzpeuwmp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jrwfeecw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nkyemufy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3scghyqiv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ijumlcxq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ovwptlxi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gjnkguse.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qtvdmfum.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ipodkprd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rxizyaeq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bcqxkesi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zaxzlkdy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xlztdvyw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kbajhhsl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cijyszsj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3munlwmwi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqqamuqs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pxpxyhhs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mdbbmsrn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bmvktsvj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wupyrbcq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mgsgrqaj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aiyvykri.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jrfirozi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bfavkwya.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vardzzjg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wzqfpqfu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sablhmze.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lvfpsjgc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zvsqwttf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ocrsyuxx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cujbqobz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nximngkf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3frmmapgb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dqwaxrpx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jrftrjkt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3okdruhff.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nltkmjhv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oteubgsp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3azqicfcu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gvslfzsx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3sqqmrjpg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ktbdagow.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iddjpgiy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bmttapay.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fsexhnvq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ijefzfym.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xvhkyarj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ikillbip.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3oelqjqpa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rruysnon.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3loktchfq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rqkfgerd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tluildau.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ojiohztr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tweoauox.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gntwbhxe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pqhxdzmi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tttziecg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3eboxwbpn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tgndczas.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tixfhlzz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3npotajrl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3myeglnlk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pxjcwoxv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3srxhcght.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3newearmy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hejszqch.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmrkoal.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lhpcakyh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzhvhzur.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3gfxxlnww.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gevdzskg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jtvrkblw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zjksabun.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wtohpmhs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xroestdi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xrkuwsan.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jakjbtqp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3autiqtjp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qnussats.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fhudaygv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ohdnihbr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfzylu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rqqujpdv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpizeyev.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yagphgwt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bbehfocv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3emitcnaz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hdkffael.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nnshibcf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ciskkdgq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pkmhmpso.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ceptgfbz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qhhwvfrv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ddguyjkp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lungsccv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sshutnha.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cfwfsxzr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sgtliyfi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ussxksbr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hruvulfz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hihmlabe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjshrdkw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ggemsnpb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hpujamyz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bquqpken.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wunxawbf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ltewkkft.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vfzxaogj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fygjmadx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxepieui.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epzopkth.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3awcuwfwc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wxiemmrf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssufgkpr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mmwbjmqb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3msdecgaj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uafqnpbb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eidzbnln.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ofykisph.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3cbhawpuw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zlvjoqdo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fegzxvzc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rffzkvmm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xcktijjl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxflswes.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ysrutpvo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3luibdaom.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jdusiyhi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jgkfcada.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhhsxoq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jnbjhpyj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zhpexfsj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uixtfvby.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ibtwrzrl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pqpurvqk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bneskqqq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pnbeagrq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aqdeozjy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pymszkwx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kdlxozun.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jiswcsxi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vvsnlaqs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3whpeyzly.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3usjyneyd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dufgcxjf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xajgnhfi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wqkrfgdo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3atlqguzk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fdmicnfz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3itdhphcs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsxetai.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vzkqszxq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xjygiclb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cijykidj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kannpkwa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ymitafyg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bqsaywin.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3roinvlqp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3clbfqusn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gdwljtay.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pwlmmpdt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lkjtjvha.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xdlzsdvi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hnyqwaop.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzumzhs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cstnikbc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fxjxaino.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3whwhxkvf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3snhpmyve.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3igoabniv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rgocjtbl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rcfladep.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3guvotjuy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdirbul.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3javbzjdd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3actbcqny.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dhphcutq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3suzozocy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gdobawza.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dkylkuqf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ysbkvohi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zjusarbe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cltqdqii.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hehciumy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekbzwcvz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3glfsxrcj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mvufcpkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxnovaae.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqicmtdq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3javnkxct.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3stedrwtz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dnejsufq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uiddkrwk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdzckzk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pooeslpu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jphyouyv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mdryjwxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdhkmuig.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jmgthlhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkljcdbm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isgngzfu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ihayrxbl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pdgbpsit.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3naalagpw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iscqupzg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rfrptmsg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3utobflds.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ehjpcgei.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3whkdhnnd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qkcnofxj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wejffnvd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pzdepqwj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zotqmhww.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vonkvsal.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gkdvxmyq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ubhzuqkc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dvdsezjg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3iogheeku.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kqeaefze.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kgijryxs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kthtaamx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ifcetkld.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iwxnoost.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3evovyvkz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pixymmvb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kfvajrcc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3anjchaer.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tmwoulux.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qwyvpxdu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mcrewsnp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zcoqeyrd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qtbjosxo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3njwkljbs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dzbyeijl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nzipctut.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3txchejos.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3lrjpbezl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3elpfrnoh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fgimlpng.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qxskbvyj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ypghqqmb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fnfucpnt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wqnfvxso.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3twmtifjo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hkvcpatu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ydxcadqc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3shmnopxb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3minrzoxx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hciseogx.html


<!-- 参考信息 -->