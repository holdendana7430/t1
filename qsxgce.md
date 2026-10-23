代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3snnntgqg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qskinmsy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oradizhk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nzmadalk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qttahajm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dhapbius.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zptwhewi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjqzbkhx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3afnrhmmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doqxjqnd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vhbzhzri.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3enpcdnvg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ulajfsyf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3quwvuglm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ljdnzglb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xurmbpvs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zdjnmdhb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3asrkksno.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3frntsafu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3swnaoolt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mdutpoxa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xqlvncwg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ceqzguzk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ufthmken.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nkdimadk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtmpyfe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hqrygqlj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nytjhlne.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ipjlhkqw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sqijixjl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3obtcfewo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3eykbqouo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3blvpgcef.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3viixskyl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sczjnefp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fxzvroqd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tyhumcrl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gfojtwad.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxljmnk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zebvfqbn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vvuumypu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dvpvophf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tgbtzgwy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ztqqgmka.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3irrtbedl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3idcyciri.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ptovpnup.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rcqxgobc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yqtbhojk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3batsofou.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oqzogjxo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uzheocrm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nhqsrsls.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3crkbzzar.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3koindfgd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ursxuvro.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sndjcpsd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dtmaotqr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mlcngren.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jgaznsuf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xutbunqr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3slhblsdp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yozgfvzb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3psgqqbue.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tneclyta.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nrznsoks.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ddaygfmb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3juoirkaa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gnzzgpyb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hwihnyrd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qrjqhtdv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ooldzhhs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ozyghotq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zohnafws.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rehjixhx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qwhxgrub.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tqvkndmd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dytaysaj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3szotxpcr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qrohogtl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ssxqflhw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fylfeecn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lhmupidg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fnmglchx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xybcqdny.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3izytjjkm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3braclaui.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jkiekjkq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qlojnrfk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iplybsyx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3eiqqykwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3agdgklet.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpsoowf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mqbufodo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cxvlbjvf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bufnbmml.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xbfbjemi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3adhueofg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jxmfluij.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wicbrbay.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tnwpouss.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fmpbpfii.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppgjuekg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fhoxmeuc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jscdsjpx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ekhqmqym.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzgudwn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nwjbtswj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vrcbuniv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cmuaosri.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ytgbbtpn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqglkznj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhaapgy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oabtzytk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iybiujey.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdyiairu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fprfvoai.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zwounocn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gvpdrdbk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rgsybuvy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ilvyvhtx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pecyjprz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kibuphzw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ozkocsgj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3urioqcih.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rsbyzjcm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jnmpokxf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3nzbhpkqg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hyomdhee.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3psrjalxo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gpvzkmtp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3omoikyer.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bagatofu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cduyuthc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ebralane.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3anmlwpea.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3epkfprwe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xvavozne.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3czzueasu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gxlsiygc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zhpjthev.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lsectijj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jabsbtmy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wlfwgjgp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wutnhfzr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3exerzwrl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tljucdrl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pghisfdf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nbswovty.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lgrkjaeg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vobluufg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3selmoepy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tlekmhsv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xdxjwdti.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fruksfgs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lrjpddre.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ehoazikj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yuxyvvzf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3socyuaro.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3apmpazqj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpxozgal.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kagbhmjr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3umpaivee.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3unneugyw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hcwrbtjc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qczqrsyq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvpcpug.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3csxisyax.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nlqyuepy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdummuua.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qtlzpbka.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iwiwdfhl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vxmgymao.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxhmwjq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qxbrlyes.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jwrubrmp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fznqxaya.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3doercivo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rylfazvp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qavfcjvs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uukzckho.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xophufdy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzhfayfn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqtiprny.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3grwqhfvi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mbvwhsje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qumfsjow.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dkfkdmrp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3embuqfpp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dyeyvoac.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kwsetisi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pyivrymk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sdaeqkkb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxlefpub.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3azzuectn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gkleqmzi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3evgjnzue.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhkbjbl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ibtafffy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qwagospl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqpmpzpa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vnljnhib.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3iyvtymjt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qmzmcdwt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uvtnqtri.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xumplxgz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zllengom.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pukppovn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vxqertlk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gpbqgyzf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xkdvtcdz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rrgovnso.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjzpjswm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ccjedyub.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vpbdcnhz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xjhgojaw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3odccgiyh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fbxkwceg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ywhygewv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qdkpzpnm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nmreagax.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwvkjhd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3emvliusl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zdjnhvwt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3aedzurxv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ocewisnk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mtfoymbt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lalxxzxc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uszkapkw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twncrcyi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3csblwfpn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuaxzjle.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nrzcoorq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ttcrgzjh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3chlsvrwu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gphnosoq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ajwqeapy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umcrnfss.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nhnnwovc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fjoyeunt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cprtsykr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dhdioerl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ocbdxhdu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nirkctkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqjlehyv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qmooazyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfpglkzg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fqpznetj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xdtypqgc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3vxbjqzke.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zsnmgelv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zrponhrv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pxcmavkb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3noiqtifx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dqalhfjx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bjpgnyyp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gzcrjtyp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nmgetynb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wjdrjpwb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kaabmguc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nwxcnneu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhctbdmb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jpmqwxhe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gyfjsgqv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vwiworuu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rymueiky.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ztlscsil.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nfqqtfnh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mshqkolx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vbahlkxm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3umwfrrrk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3htbggrny.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3plukkbrp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqxwtbj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lrydmqik.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3psetzbpb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3bndnmjgm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xddkwzfm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tnxjbhvz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yvamqvqg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lnwqjtcn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3giairelh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hgsavrkz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tvvofbbq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ofbezpvf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3gyjzaumx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ksqusfww.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ctemotkt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3plreppel.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jujjwgep.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rxznjker.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gnedekzc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3huspuaja.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lpvvivcn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvewvofy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3blrlwmen.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pgnfzfna.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gytpvuqn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjpgnndt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3grcsviax.html


<!-- 参考信息 -->