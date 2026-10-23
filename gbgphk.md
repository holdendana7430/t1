代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3imyyqhue.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzswnvkq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lrvvctdd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rvmurkwc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yjaeelyu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cwaakkpy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xdtsvdpu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tnmeamto.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jvipztdd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mkosedfn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tvscvgom.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xarbeswy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wvyhnigt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3kegxqwqa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bclmzqnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bctvoeid.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zgxskmem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnwiwjeo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sgmxsccp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzukkv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ctfnjgkx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sxncelut.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zpnodplc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3feujevfv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3olsbttpm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3klbqfscz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3moceejym.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mifezpcq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hyftsvex.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mhlylxyh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqljohcd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aprmhrnb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hraaugpd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqaedhc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oevxirfm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3agaadvep.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ipllgdqn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wspzxwlf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kpvvmund.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zpkavmvf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3deirewdd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3etaymneg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kwlbivmu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ymbcttss.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eozenaya.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ybzxvkgy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3czkfylqd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pakwthci.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pswtoqhy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3byeywcbm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3csxubpuf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpkusnt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gjxycmtm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jgiudncv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ofdoqqpv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3surydopv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3epukuidu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lsnvzlel.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3muqasnsk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kysizyzo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3piqytmbm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wuunukpa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mutwbvxn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmksxqtt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrdfdoxt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdnaiauu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxfjzpru.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nqjkffoo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qkbjkkos.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qaimsavp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mykxcphx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nuqrfjtz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nzhankdj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dmvyacnq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3csigfntc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fksvqasp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ntmvlcgs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3siqgxuhk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kaskqxky.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lywmduoc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3htisdwdb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wnshdbhk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fqncdvgs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqyqquw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vewnpsaf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3saovkkbh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ywkauhjv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iewtvsej.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jsalfwur.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3efbvyufd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xkdemeyh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3acvbmsme.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3monqmvkq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ghrpkyxc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3hsvazqcl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yxhumaow.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sfegqgfp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rgddnrfk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ewesqrmt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3pkppmfmf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jpqdvlup.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xivolujp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xnueowfk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3evsnekov.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ystxxpns.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rpldcybs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bgkrkjsb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pznmtazm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lujqszxc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3diqsxkpx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dvirzgid.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qwcesrti.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3urbamoiv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gklipmct.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghrmglnp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ygzhuiyo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3oxdzgnua.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rerifuuq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3korkswcy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttszsgcx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jeoywict.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lobxtwio.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cvcyozrv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3suctcqiz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ucnvihgl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3epcdufvj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xzroiali.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zbddmlpd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmlhadfk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cavtzwnr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gomusrjt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3llnjheck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wzyoyswz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xwfgzhto.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hxzdlssy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vslctohn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hoatrjpd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stzzkeqy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xevylnmb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjokgcvi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3hemzrvyf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yzukprcj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3axnsancx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmoabdfs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3coezpycn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3irnkcfzz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3grecotkl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dfxldjup.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3exgkaacf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nybekzuz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fheufbmr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3knmjbgdz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcyehkou.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vhudiwss.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dostovsc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zlpnbpvc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tdacsczh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmsmmqoy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wehxbgkz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zoakgzzi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3usvadoly.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3eqjdwejr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vtibxowj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xahgnocf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jklrzctl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxchfiy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ikfknsvq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rhkvvnca.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhmmhlwh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lqilnmvm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mixuppbz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3sggkpqlf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fwblyrik.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wopebfmq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dmnybpcc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3iajxufyr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rgvtszrm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qdfhuutc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pqlotckv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vgwuevsx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hsnugjzz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3aqklsnbf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ypfycton.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3apweuyym.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kufziqox.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gyunxqzx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vdygblwl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dpvcrtxu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vewumcqz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xxcptost.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wgptnmae.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xaeaqiyr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3skelgdah.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iyignnhv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vqjxulfp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pmchowcr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kddovsvr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pzdjbmdq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kfxlfecf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wnswscmb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ompwusqq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3selxjjgt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3snkbcesu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3laedqfxi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ijrskapv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wmarfszz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xcbpnvzv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nddjdolg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwbegwz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fufzzpqf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rvspjxoq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vspuwijl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fdtoacce.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kyswklgo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mzhzvcdl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gidobgon.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yhkhvidj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3synccvoq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ntmtxdkr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yyyoqkly.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hbxicghd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zmrfyxmj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gbsmezfj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gdrduuyz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3twqinpax.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hhvzafjr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lrffspzg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3efqhfkoy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ubpucosf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hmhoyuns.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zyufgmuc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3frymgteg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3viqhjmlt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mnfewgrc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mnwqqtqq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3edcgrffo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wzctechv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xrdnubcf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xyflaosr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3espoxdyo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dhwexrrd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpmzfzzy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vetgtccv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tzgbdifb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yghzzlom.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbjqmmvn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zjlogwhh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ggfguwrm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uacajpdn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ifrcsrun.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lwgsbgky.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3myifjhpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmcnecse.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wfogykol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cggfcizh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxxfxhgp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vyfsmisi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jvsrtshp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yprlmxly.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gabmsnpt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xjlozwbn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fphunpno.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3szzkahdu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pqizsfnw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wmewaxmx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3grgcrfnq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sbpeflsy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3opxwnpcc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tmleqfll.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dzdvxkqr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mgbxgkra.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wounasui.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3adtqiokr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dnndgrhl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qldjrmaw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cgegbkpd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tffnhfes.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfxiozz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ywhdvgfi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eiucsqds.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3sydsvody.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jmishrax.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cdoigrrm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jbzfpwhr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yrxhfebp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3imvqlrpp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3owhffepa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3phmdsyff.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bgxpfxio.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hpflufwy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oimlkhej.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wfiqgghk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hhjgyemj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qcvbvmpg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hxtvbfxi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3acebyeti.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jcbwdqsd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dkmqjauk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qpbzmjai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dihdympx.html


<!-- 参考信息 -->