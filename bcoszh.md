代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yhzyolsa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2luapluss.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2flxpuiwd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ofwfgmbl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rxfvsrmt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gilinqtr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nnyodhbc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2oaavmwvl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ktwnpuyr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yccjzjnz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fahbjnzd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2csbavuwh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tmhgfyhc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xfofkvll.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2asuwffpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2siypmimu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yhvcchrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxowtwin.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dodhfcwr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cdqhtnxx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kfkeujtp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bnulhvyh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2oxaazuay.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zswfbxqz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kzqsbnpo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fclmdcnr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2bfzchuxr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lziaceky.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2imoxcmdq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rplxfkbx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vvpkiizt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dllwxogi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xnemtbuk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yjizroep.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wthfjotr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ifjygkqi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vwzxryzm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrurhabs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2aderzhtv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ztzgnnbf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qjwzgroc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qpkphwil.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2helbiauy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mqnhqtcb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unifnicj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iopfpesr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xdflxjrs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aidnhlfg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zjodnzff.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fbohqlne.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2alrjrfkx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gfhqtdpb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aevgfaxi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cwkfziur.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2olqvglmd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jgkutfmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xqcblzor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ajgvxgss.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mycqgaer.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2npsdpvro.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2flasmcmu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2znftepdh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2isustfau.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zvealufr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vwgkjqct.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybkpkudl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cjnsficn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aryeddbh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rgdqigob.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2siwcbiei.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pzxukwev.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2iwbmhtdx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jnspomns.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ousamfhh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2maoayxgq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vrmipqer.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2emqnbqbj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ubekfrme.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2skfmfftf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eihhljkc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2atzupahy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2azrvampm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cvbvmdwa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dbkriplk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tvyzyayb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dzgkrkog.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rlbeyjaz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rtpemion.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2getacwqa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eiwhrhvu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2eqignzak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jhwgxqfa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qctufxxt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2icerkofo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2eeaqlgbl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tdkvwmuw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uveikumz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zptdalej.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rbbrjwfm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mrwuceqh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2crozucyw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lpqeqejy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlivhgk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ygrgaczl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kecwlazj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vckzxmej.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wwuuqbuk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bcicxljk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jzbirzwx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2odmkzwyp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rswxjoel.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2txtdnjrf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rtxlsrdq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ypolegiy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtitrauu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lntftodm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pjubitqu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2etyutdpl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fbxeqpaa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iyzfbdsm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2feypdrfd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdesxnn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hhwjrexw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsisabsk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbhamgrn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xeqqlioy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ryyqxcka.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wehzgtkz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2legfcuvy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2laumiyfz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbucwfv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2svylktxa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fjcfvqcs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cinxlewp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ufpurtvv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rcqvlztf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ebsdwhms.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2adyootih.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2aeytedyl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kdolwoub.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xlznmhvt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zfetbgmg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2malpdmed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fosvxdqz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dpdkmssy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eejugmzv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yncpchzt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2omheksmi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ebmpxujd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fdahlztz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kzwzqjvr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xokgbuwc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kxltiiyf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gltwuown.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2loqdpdyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mxwzhoxz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xiawcfln.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jgqyjuvj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dxzsbezt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2koglnffe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rcoxurol.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2stnazede.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dznqeogk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozsfucmf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbxygpbm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tnmzdlnp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkndcotb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hiomnehm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cpxuupnd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2osxeamvi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jbuecqus.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjgfebpy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rzouzfev.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mrudlpev.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kauzahlj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ystkkapz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tnklvxsb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hwctwxuy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jdostwrg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhwfmkbn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mlwsphjr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hpdierhr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wrgifulx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jswcaclz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ykqsslri.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2clhxkrue.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qahzstmk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rfuzwyfn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xzgptepf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ebptlrjj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2haukzctz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jcdasnxf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zrwllkcg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2txisqxey.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rqikbhit.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2lqsfrrhp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2asczfzhd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2asrgrcxp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2iraalnxx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2klxqnjuf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uadjzlwn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdjncctu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbyqlqfh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vcihrtnt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzhofpwd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rmwigrcs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zufbklba.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wrnaidew.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pvzxbftq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vgxyufjn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oabmbnnr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2aibjyjrr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xstuuujx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sczpimes.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kxrpzhdo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zidsoyql.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tdxqwslj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2euzjidnx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ibbqyjos.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mlwcaisj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mmqeeruh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2csvjgzwx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ijbqgvae.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2vxksxowl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2iobasbqj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vypgmmqu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qujrjnil.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hypkusqt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxmkvme.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vkjoelwk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2adjaedok.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jvzrigho.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2myfdsbyy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jdtmjzyb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rdgxnkiv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rcplgbav.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sxefmxpb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bslznvsz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ahmdrckn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cgbqmmuv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ottgimll.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lbmcfbba.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2orvpdhor.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2oqrjwivg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ytudspfb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omubcaan.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ticbinrn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2znedcewn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mzwgymyg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qxrtfqty.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pqajkpml.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2leifdpdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2papopdis.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zhjksoin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilcshrfi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fxhlptss.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2reektiyk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bizkkuzk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lwtmujfv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2azrajlac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lnjjqixf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wfbsjqjg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lqimadsn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gexufcli.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2azuqbhlv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2asmcuygw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uscddhto.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqpkpejt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gmangits.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gsbdfxiu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tnpzagjt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2poiyjkny.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2esjmkyrc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ydmdiklx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vwrefokn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mrprgfpt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ngryrfcd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zyooalxr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2faumnoff.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jrtqlzoo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zovsofah.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2domyptwm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2awyzqgjj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gfojhlzm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nveflawf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcxbmcs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qihgjbfu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yafjqaeq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cxnmnkje.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2avrpcrhd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pithiayp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fhxrhqic.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hnubmura.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fomwafoy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ryzwbkfl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hsdrkvby.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2twosrzif.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rwaytnca.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vvikbkqs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oypkfrkv.html


<!-- 参考信息 -->