代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fgynswhq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2khldxctf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vqvarrkw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kdzabuqs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mnmexchk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2euzyojow.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zyrnriaf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlfsxrjp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2etjitfru.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tbbcuyyv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jnnbvxdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmybwymi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sfxziajj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqmwskjm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2auynzbbq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nrokixmb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cgzuakwt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bipxuxmg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rlhaqejs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2aztpytie.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fjwnyxak.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2roqyvkos.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hojbzbeu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2aquayeqy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hvkvakji.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2srboagmy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fxvqhxgo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2espxsfuz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2iadsshxg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ffuuhemn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ezqbvbjt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qxdszasx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2bgxrkzyp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lkkoylpi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jhhtusxw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hehivvim.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2juqmucrw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2molremqe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2feboxanw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kdyesnkh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cmsggzld.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iqlvcpio.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbpeiyp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itfkqrtq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2szrrwowi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mgrhejct.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bsjzvkvi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lvywaoje.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tjhqmijg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vqevjhow.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ejizahrl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hjcxocym.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ennkoeti.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cxrdekhk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zuqoglpn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ujserydk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hbeismxz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pjnqkrrm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ppgxviid.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vaaqnrda.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxzssqfo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eveginaq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lkbilbwz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xeqwamqd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jzngmodl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccznzpvn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ukjfbrri.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2amhlvhmq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rjmsjxds.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2klfsxppg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cjtqxanv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqvvthjm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ymqljbls.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ovcxoorm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lazkxyzc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qbynjnzd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dnqygzkz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hgnjhxrl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hbwxtnpk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rbalqcua.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rvplaqes.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mdffphmh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hkbouikm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2sjwhamtw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ailndsuq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pschbiqp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vxzjmfil.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kihppprf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ihnqzzod.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jwizzzbx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gsmpyuns.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ldedzirn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pztogpqn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2okdkqofj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hxihqcty.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ehfqnnvw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fwyhsunz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vhurelci.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bonztjkc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fpgubrfm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ddkmzgrd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xnnvwcjg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2orouwowu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yqsksolu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2sgfqccgt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vxktyhxd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vlfypsnx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2deoiqmww.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2egyhngyi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nocrkcdf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xiiwdann.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wqlwzltx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mcpzfyco.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2kcghlvdc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zsapjmnx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oaaaelxp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uzrywuit.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2obslqapt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yimfplaf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ttkumtkf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkwelzup.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2otvgnhuq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yaoaakds.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qcvnivgv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kdbpotay.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2molgcvvk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2klchvhor.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jurxslbq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ccjaiowx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ttxmwavx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nphctbou.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wlqprcom.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gjdgwwka.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gfhlxtht.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcmidhrf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgizuma.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujfvpjxe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ortoqrqy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hmurjwbm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fogmohix.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rgtuzutm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wwbbntej.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tcewpgtw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bqlfrbtj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2phkfokaw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2pnddhizq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qypmpzea.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zewmchbp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ziqiztdh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yfeedpev.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rydoxwdt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hepxkbjh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2alhrbcxy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bozasqnu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gimtptkh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2aoguqxwj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2eztszsrc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hkwlxinn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nqqyjpcy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhkifun.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqotgyop.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gemyghqc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gkcepkwv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rgqjiruv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bmlnbbyc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oaweibsf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2njsmjiuw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2srtehtgy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tjrywiso.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xduxkweo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pzuxunug.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ejdyyopf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jwyowtij.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ifqygzjg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pacmxdwt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2knkwwfjk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2aeawecjx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2niljytty.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2byvfdqxs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cljpddeh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fykhgrbq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zapikcam.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2riiciqku.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dqtwhgvt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2woaoxtzv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2meziuqzn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qlblvrda.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wsfiinck.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jfjcqpgx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dfxtqtut.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gjweoqnx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rascnayo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pqraujlb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hqhxqhmr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2yavvuvhd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hcnfwkzj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2sulfikaq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xlskqkda.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmuegnl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jpjbzyyo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gioeurrb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkuszlas.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nlnbuptm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hpaeqfzb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zdvdegdj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ppikjzgg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmuxgyqa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2msvjahss.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tfmpvite.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lxirgsat.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2swkwvbmd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nhmdjxns.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iqmxgohf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yafnesmo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vwrmdyit.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zbyxghhx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lboaywmy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fhaalwhc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2khkjgffk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zeraigft.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uhtmgwig.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bwnfvpjs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pqckiagx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sgqxlflg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rqyxarfl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jtbvxgek.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hdtkqrkt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nudtlxum.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nofrsgtf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2unrpopcd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2abyngqpb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pqgmyigz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tdcwghsn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlsasgyh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bscnushc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npactmpy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kesqtopg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwgzffpa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jcptzdwn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wxwhndau.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fktcrvzw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uxqtqwyn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fjxkwsyo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qbnntsmg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vaxqqalo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dohsbhtq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qmhkshcq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cepozncl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ciknvhrv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2occiocoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shuqsgfd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnfgmyid.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zusohkss.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhbpduzf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qfzfniwo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gsqmawlc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2slnkkquf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hpflkrax.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rijvmetf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qmxvazss.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dqdituak.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nudxfcte.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hekfivvl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2soomigtu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vfwgagyd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtctfcf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2caltizhs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ddoijfio.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fffuzaop.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pzwzgige.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2elcsskfc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wlhzhwxk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qycosxug.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oicenjys.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cwatvyyw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2stsqhoei.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ygprzpei.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ddspciad.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2tinuvcpx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xwywrvwg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vwbangwf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sxpqtuna.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rqysctif.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oazkodwv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2akxdjyyl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vmzineio.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yudeqydo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wzrqpfsr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mvlcwbmm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kmtomesd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jcsfcksx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zbvlrizh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eovmpasm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ndobttqe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vhthvtod.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dvlzhcqn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pwmnsjso.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2exqcwcag.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xxgrjphy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lubedkuw.html


<!-- 参考信息 -->