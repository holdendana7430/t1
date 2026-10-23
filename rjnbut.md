代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3oykewops.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mxldrrmp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pbjtjzdt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cybpasbj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fwknowau.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqxrluwi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3udjtzbno.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lvoixpbx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vinnjzkz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tiuynqut.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3swqpcoia.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3apmkedea.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dfjvheji.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3esyubgws.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kivshaoj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjdgkxnu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gaellvis.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nsbkpinh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jervacju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfaacyhd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3utbpnvua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfhcsvgj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gzjhwybv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dsdmziuz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nygcyzar.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jxdkijkg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pntkypad.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mwqkzjfb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gkmkvgxo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rltlvtyy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3usibvvwf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kozjjrqf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gkfctcuy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qrhapvyr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhdiajas.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dpeakmds.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgboxpp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmzipds.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3czthssed.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cclojfle.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3kvxjzjzw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3otxrrgnr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bxjfbajt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bhexhmwg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xxarlfqg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dvdbwncg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ivfhtogn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jvzekpvs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xnediewa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3frmwteew.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ylkhxxcg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nygjzjia.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3woepdvha.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sxoedzrj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fzxyfwax.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3myplggui.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pwusoilz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3oceczbul.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jsdpqfun.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aoavkxxe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qdexjtcy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3srapoglg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uxqcjzmz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3aivnerwf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bktkvurk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jmcwfrsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oczrksea.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hobjsniz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbwdsyfg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wdsbhbdi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xhomvgll.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zuiastbs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lyunlpyz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qybolfjb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hupaipni.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sdjyaimu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3aowhprgs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hfkylsii.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3akuqzjjd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sonlqhrw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fyviujqz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3neoyjpxx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fwmovdom.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3swaasiyc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nxcdwllp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wimqokso.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gnqttvbf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3klbzrxue.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3oqvaptxz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bkzljlai.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rfbqvddw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3buyoapjk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hvuhsjpx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tfznrcov.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qkeqtway.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nlxxjaak.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cgbnbpul.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jynogjpk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3aibpnatc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tiigwrpt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nuqdwurk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pfqzkofd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xjhccnnm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tjsjhifq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jmpjwkny.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ncpmavxv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3btxxwulu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qakzaopn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rnwyfuuj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dwabigge.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hwwygnmy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3josqsowb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3omrbpdvp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kscbkilv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjhrccvn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3timexvia.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hsbtlbob.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ijrwksau.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isqjqwtx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ouderkwg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gsuimuua.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bryyblei.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fmetkjkd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rgmjwews.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbrwgkmd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tbmqjeib.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ihherxbs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cmqeftds.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jxytenus.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uaqwvqdn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ccxdqcdk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qqtrncox.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3awpwdlia.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hyiegjxx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dabggvif.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dfmzydzd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dsadiqpg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3alxfamku.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xnruzerh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zfxpgnhj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dqiyzhmv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rlprlijs.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3igdvvkeh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnnpurza.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3igzamzho.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3diqjzvwg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hffgulwh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tzvqhrsj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xuoyunxt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3deqhgpie.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jpgqlgnh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rdgeujpt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nafijhxs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ykhsmgmp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hzwegewh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jvwtotnz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkmmjfjo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3obxdujtt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlfgrsle.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivqmkesl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xantnjog.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jtsqqxzw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vrplcxmn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dfdbrrel.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3olnyzxft.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3roaskeha.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kgnzwepk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbpvqlh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3myphasob.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3acozsebc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zspgmocz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vlgcpfux.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jptlzezd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rpdjgsqr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3loqfdgbf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3afhqhasr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3grfeyjhb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3oovfsznu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3datmrnhe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gfcnsowj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3usbsgike.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3pkwdvrbr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3elxlgjyp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mgmmdcpw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ndccbmqm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qtsfhtcz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3msrvjpvo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wsyjxyta.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nupxwxps.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dkkogprd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zqozrxfe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fwitaxpx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3blotmkbq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ktetozqk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmnlfgrp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sboicmfv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bosqezbr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yidldgfk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3kcrihctd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zwxfxjbc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3mhkcssdp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jalgjbsd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yfzwlvsq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jqbyofzt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gbsnycmu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qimcwvek.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zaueinaj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kdubkhsy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3byyrtoox.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eftxkotz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aevizhkk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lwnikxvr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kjtuvkqz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qjxbzrnb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxjmvnak.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3bjnmlult.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vkvymgmr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mfchzhgt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3obrwuslq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3akbznhfu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3egqobkge.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aeqgxymz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xiqlvtii.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbroptc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rddjyxwt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ujivsdnk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3usgkmcnc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hkhzwlny.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ehmsmojo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3heuucdqb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hsrnqzlt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bdffwinx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3emncrvsw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdnyrhnv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qxuqasoy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hwfdwjbt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ealpwhbd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wnyxeifq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bpknvtpv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kokndsiv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vahutbrv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gdpkwzev.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jesnbzjw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilglfpkf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3wwhfiehq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cxtslwzp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fwxemhsu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pnmzdjab.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uynghxeu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwyvfvhg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ncswdelt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3epcclpar.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bcjdyvof.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3osuokpen.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rxllrzst.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3brubbfin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrxtydjk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gxwekgdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfxklgvf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xivacehe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wqhzqroq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3stqmfhqn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jrwnyfsq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zfvqumcf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wqcwcdrr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ijftylfk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3giaplowf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iaqzrzcy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kwaacano.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ifibcuwn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bwavofaz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cvcnndit.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pnuhtzgu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pswwtyal.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vlnwgxpk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hkrviyka.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kucdqcuf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wruwcovx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uiffvvjw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zpcjvczz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3phjzwtie.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3irtbouec.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwdtbko.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xpycyeik.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3walwrlym.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpocbvs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dondcnad.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3crlzajsu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fbaglnzd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sbudjrpo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uozxcvjm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ivkvmxzg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jwvlqlbq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eggrbqhz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xlpoiaim.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pfpdtvon.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tzemidqo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qbzezqmn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xfchtqnh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iqldiztw.html


<!-- 参考信息 -->