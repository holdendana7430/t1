代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aqnibqis.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gimkqgbe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wbraykrn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zjpqoawe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vtiplcjc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3celgjtid.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ulerhmob.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gogeqhgw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3klwikqtx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3cpbskjna.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3txmwrsnn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcleqvag.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3sskhyuim.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3meplpeki.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxcotmvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brizibqc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3javoffio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiixrudg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3imoqavys.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xrvnllnm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3empcfcgi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fxyousfq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wneffwkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jyxcmzpl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zwnhkjsl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uqswhjwn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jhkyypqf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dfaljabj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tiicpcys.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kjxqvuco.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gtrhqekq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cbfsudap.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ehmzfagp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wigpsski.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hbncnoqf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dsgbdcwb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xiyizmii.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ixpblgrm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3drmyojad.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fcmqripb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nvgwughg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3buhilrnj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kkfdspej.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ygglmbgo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ktdirnep.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ydhafeha.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wiktjqqw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bknwkmkh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wwzexcmw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wzcqlxld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zlckmxkx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmxvnbf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bbdwzoms.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3phwlntfc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3prsehkbk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cwfocmnv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3udhqhidt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hjarpkiu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3sbzhjtfw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3swumrcdi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zblkbcff.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pibgbfir.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xkvzgwzq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dmewlttb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3izbmyree.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyjyjsva.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nzlkkwmr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xxzyorir.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mpovyzkq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbicxstl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ofimzvsd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ljkfifhm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3psdbgkuj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3aarlrhuq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yudwlufw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ynzvgqxf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3duqezafq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jzsnwpas.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nizrofbo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3paulsquy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pcopmzsw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zalrrchs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysayoaxm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3finmkaem.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zvmgywpd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3anpncdyt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orvohbwv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nluruler.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bvpgqadr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oeqfajmc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mowoinhh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bumotest.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bshfdsjj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jjkhzsmt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3pxybyycq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kzqzmtbi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvtdfpde.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tpjblrhl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jraxrchf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nunyqwao.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmmwhkl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxuvxlpi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lanhmsex.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ckzzhmpd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3npaujnqi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bnkwkhmk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mnxxetjg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3soiqvptk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zhbzkkgm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qisjobfn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkdkaoqh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mxcyvbon.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3peqdjzyu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kwciatyw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibizboep.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tfdpxnpo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rtdytbca.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ibuxanrt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nytixtkq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pkejlimb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ehuhbnee.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qohvqhif.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3khgsywlt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvxjbed.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mehbhwqb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fhnejfjc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3emdredvd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dpabdntv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ddetzjhu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3stqdfrog.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ylryqdnb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3btyccdky.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bhzhxsod.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzfjkkvp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbcubrtz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hnnojace.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3edcobsnb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dshonnvw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbnzggwu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ohhpvsqr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahqpcsxi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rfjcgjwo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sagxaduf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rcibpyfs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rskrjftw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fdwnsrmr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hasietsb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3absvghha.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xmlyexhq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cqycplnm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wwsclzqt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ibsgbqbg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jrenlota.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hnsnvxzi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dinwdndx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dmmulawi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3medxwhlc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nlditkcw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3hzqgoyis.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qpulouzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3skskgeot.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qjspabke.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iekuxaue.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxmqczqh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3yqdmczub.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bpjjswoq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3humqqeec.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ifwzpose.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqbnisyb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3abwbpqap.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3peikqfpj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hfvmynfw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3eoyvkxwe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwmvtor.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3aahrsthy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ayxohqhh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kmkdivmm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nncqnddd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rdkpdcbt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lovghacu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lidpqzui.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hgrblxqa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jajkhqzs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qlpzzpjz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dydsbqjk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3caxyvlih.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xagdouzn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rufwmrfa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bkqktqse.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kvdqzcnu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pybmqphz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qwunpxng.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cazdickd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rwtlqfec.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rnqbxpbh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3klkvijfe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xgvvveig.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rlompaii.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pzoaexmx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hblqwvmw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3miknctrw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cifjglia.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zvghgcso.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dcfuflld.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3anuklqos.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwkbilqd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ofcijiyh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zkxfmqof.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vygcuwmf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3miqkbxcn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ltufrgzw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xjezklrf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3owcvofbq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3whokicbp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qdecbuph.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jrhnlmjh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hcfwytor.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iowurduq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3acgdkbni.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3thzylhwt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vvsjfzif.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3raxuvmwu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nwmrwmtm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bfbcrqqk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3clorqpac.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iolfaerc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qxjjpebf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vlihlfqi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpvjqzg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3knmmrddo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ohywyrzz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rkueplwc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3djcwyuxp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kiawmwqz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jdgboszy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3quebmjea.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3grqjcbtv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3awqaqjqd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zmmauyxy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qgfnshhg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nnewckcx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jrisnmai.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3otwhovql.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hhhostsf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nqiufpiv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsgoqyxq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zwoidcxh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3grkdenfi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3myrqqkou.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ycyhoung.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hankpzpn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dtsiyygu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bytlvarb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bmjelavx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtyobuha.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dawbgeqd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oyyhrdri.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oebbbpjs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hpumsczj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgkzhfrz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3talryzcq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hfxynbxo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gkzdnjjp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3otbzpida.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ndvjhzlo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3krfwkpnv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmtnkcuh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3orvtrbbw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nirkanlp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3satkqzmt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xcakblul.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dcsxcvtb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zoyqawzt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hctvwerx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kkqkvgrq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rosvoerh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmacpnog.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdhayok.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qumvejaw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3udizvfko.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lyofyswd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvusqgzz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yctgmpkj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zcbgdphs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xbzekssy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cvsspllo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ezflvmyu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fcvewrtl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kzclyixb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qfszqeft.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ypzkigbi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bqkmeqhz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3csjenain.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mvzotmdm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ewcooksd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bwxwwvcc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qdxxulto.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fnnwjbzy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oiyllqso.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3prduzwsf.html


<!-- 参考信息 -->