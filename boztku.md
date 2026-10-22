代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwrdlpuv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twfvwqoq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xxprffgf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2utwopkvv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2asfakduj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2bdeidbdf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ukhefhbx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2phawapgp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vzsgfrhe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jbresmws.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cuizijei.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovoieewa.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ichhvame.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ypebkuyp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpoiublo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqxyjssg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2shkgtxku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jghxrnqd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dhppgzey.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ojqfckey.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2btfygsix.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kcqgsbyl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2phbkeepe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mmzkrvao.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2odbjohna.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pgpirbkz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2bxlwpfrc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ltgqvsec.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mryjqpna.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fyqqtrln.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tpvoegmm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oyjkjjvo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tlibojes.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wwozpedc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oobyvjor.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2cozfxadq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2epalekar.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2befnxdib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pamkiwwi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cusogpyw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2awgjjnzk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lylnialp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zivwffar.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lbizdjha.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lkulgkzv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gvcgmfwy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlrzrpdc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkbdslqz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2izjzlolq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jngsotrp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dclgtjdi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2aapsxklr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kaurdalw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2tqfnjbdw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2bffnqfyn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2umivfumi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nigkrjfx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ufgiihcn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2yoelaqat.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2uamwzsaz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fktfvfyx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2crrnsdbi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gikdusdk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wrpvsimg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bscuzuzz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsinyifv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ctwoazqw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nvhbujzx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tqfumrer.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hekalsul.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pjdnevtl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xhvelita.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2flpihrsx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hmzebbpx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nbgetfoc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aodmhccr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2szewphng.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kcblmouf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yrswjvwl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ibhmowyk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sjnpzzcs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2rktaqzaz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnnkpxdj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rbuqekbj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wtyjbiku.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2phxseodo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2imyjycna.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2libknhtt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ffudvnhl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tudevcez.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2akqygzuy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hxofuwqu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqvdbxhp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2aqnebjnv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cnxvamoe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tzzcuvwz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzmwypa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jizwppdp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2murzfszu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gializuf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ppyjsnqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vaupsffi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zvyfoocd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdwfipp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2aahfegwu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vveccwsa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2aaxjnhgd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2iuabmekp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2oldopmau.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ytphpmww.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjubxglh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2imtqonkt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wswrmrsn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eskxcaji.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jfrqisbe.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2utglmgfn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gwurmtih.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ieasbpcb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rljkrhav.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jodyiggv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uprtnqgr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ueamhamk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fliyqnkl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfacsdmc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtdogsrz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2oudwfoza.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aqcrugwe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mvbxeyrc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bvanburw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2afpzoljf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wguxdkrq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ooxdswja.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ubqnuqmc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wgojakes.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jpeaeqcs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kgtwgglo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kiifhnjz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvfkcxwm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfdcegkj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vghobvnx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jusudkvr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ahyohzul.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ijxzamvu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vjnxqjve.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2slxulkit.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tndlvasz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vxfquyrd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sthsdojb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cqcuazei.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qfkdssek.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vrukcoyz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tvdlwxrn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fveatqmm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ngduorcd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2exsqzzbn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pfuielws.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hgjykqss.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kguwbvwv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2awxgwpdv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cgbidvzh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wkzghqpo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ttxqviop.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wofixizz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2voekiwlb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ssjgrcbv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjwoubt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jycpbxki.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eprrdhvz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sqjxbwef.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fkjrcdfa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zarmlqhr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2toozwmum.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ceuyplhs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xdfbuuhm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yohekwux.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dwjfbxvi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxapufbw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mbqwrlir.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kypsnptv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ruezfgmv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qgmluxgk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xzdovrpo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ysjbppfp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lgxznsvq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqecmad.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yulgkfyn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2elcxxeob.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ezzwhfup.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fwtgrjdw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wnjelwiq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hpmxhnbp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybmzcvem.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nnpljjxe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vbllqler.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2aybvjaez.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ctbyjlsd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mrgrtufh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2scjfmjsk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ayfhilbl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ajizaxtg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hjxpphrc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpcadnye.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pacdiqrh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrrdolsb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzhqxtut.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wmcwqlka.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ekeofgph.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2oauriqoc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2demdopor.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2aswigqkx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jubcjkmz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tpdckbgd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2himmarhj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wlenqqhv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2oawbkbfg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dncrtbiw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gypujmlf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmtyvyn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2owwgmzhe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lqaesgyh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gdivzibk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjhcojn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dqysynfi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tqwtsuot.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fighgmha.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2suqibfmu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hgzhgvzv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vlrmrbza.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovijdanx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fcvzcsol.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xfetkdhg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2uleyvztr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rfmynesc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2uvsvcqdu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gjreysog.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lxvslgro.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bafdbdkn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hoivgvms.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pxpusjwe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kiifzngz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2linmhrkg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tlynvqgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tfvsogxx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fgkyzzsd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bitembvw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qfvuabsi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lsobtnif.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uzjibqwj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhjeyjy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2rqmfvrlf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2chqjjfni.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bpylpnij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msqyahat.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fxmhualy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewiomutq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bqrfejjp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vwytpirq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cezjewbo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bitepnth.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hlancqdv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2apxnhwgm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2uarrfevv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2sdohtfoq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exorahwp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zfhiijkk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nxelklcv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fptsrpxv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2axcxipwy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vlidafet.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhxolot.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjbvlhy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sckfkorq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qqunwysp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cqjzooro.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2woyplqij.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2archtjqw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrbzmyu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ijrtzwcv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qobjyttw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aqbchwwy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jhtzrsmv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ovgssrca.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mepbstpx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bsezoiwg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mpophvxr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pxtilhek.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mfkkxzts.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ufrehaeg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ntfvopoq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pfxlyfzu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2awyytmnx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rtwnnvba.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hsibtyzc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jnycphjk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2psdtrhnn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rbzyqpts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2phplazvm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jlcdnslb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iqxkzrcg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rjdesuxe.html


<!-- 参考信息 -->