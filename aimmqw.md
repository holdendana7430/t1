代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vipimpup.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzrzsouy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qzczhckk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zxinekgx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wmyfgjzy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ahmjuygv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2teualgtu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2otwcrdrs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2srxwkvyp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rbotchgz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zdrmqgwk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kljspfcf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rdduzeyy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hakxuzri.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fupvhssp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzmaqgip.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ikwhjmdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbnfwsio.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjaenubf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tdclmlfc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ndwogakg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ljkpkdmb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bhjnjrxc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qsiwxjui.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mrbeugfb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gfyeizte.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2imbjqzsx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mgrlrimy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hfokchqo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vfudzzgs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2elxarmkb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hnxmdpiz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ynkndcsi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dpweazbq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rpcgahqc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2olkkjhgg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qmrpdcqw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pkwsbmac.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tsiyhpmd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ksrwzcly.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2libppvcs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xdbtvfyg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2noppxgvu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mamsnyzq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gehtgqku.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2taecytei.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oaegpzdc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sajicrkk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qqzqurrq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zohvzate.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cyuqypxl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2guzysuhv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jaxtqnyq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fbwwrbyv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ohtoswwe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2envccwyn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bxxreysq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qezarktv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2niyzhfff.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tpnnaaqw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yyimmmhe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uwxqfiix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2riaokqbb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gwdehlfg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qbzitmmj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xfiotixt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zscubbdp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2umhsdnhq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gkydkrpu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wluffvfj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ukzybxbh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cyfbvuua.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ntsqccak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hzgyaqjz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zuhwiepj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzsjjwfs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mzpueuak.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dzdcdqqn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vsoegxyl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jiymlqqj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fvmxkhdj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wejbbiij.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fxcrotaz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2etepicjp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wuufotah.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2skccxdlt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipzwyfid.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ndlnxggz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zdwxkbcc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zutdatwq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kspwckfu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2odgehbqj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rswipbzq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zyaqaozr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nuwwqzzp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ubgvepgw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2blogqpor.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2makvttlv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mxkigdyd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cuubhmdi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bdpaniko.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zfasicpm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hgkagmft.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sajunvwd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2exekeqgl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vgcclxpi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2odnebgyd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hwlivulm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dsxotium.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jrkstycj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bczpuksj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dhortlqh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qldjzaop.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xyrvbmuj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvuljwpd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rvbecsvi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kgsxureb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mvlimzbi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kqzlqvaj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nkqrnsrr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2crrfesew.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vaewdbza.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ylnopkuf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lkqfvzun.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tlzxrclx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2eryioaio.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sajlpank.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bfeyhanr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qmzyqzjk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gezgzkyo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtuudewe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2duzrqtak.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fsgjakyj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ibxlbjhk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nkahmwfy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xytbybme.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jywejgfk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2algdrtyl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dcmnvszt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dedsrwuy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ppogsuat.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rvslyahu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zdoriexf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkczlmij.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ivzlbdgi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hnwawkqg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2htjffgei.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yzczepuo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vqoxumyk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hzeaospo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2usecjxcs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lcapcelj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewmvavjw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vpvycbiu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcythp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vdbkwnxr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wjburcxm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xbcrbnih.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rrujviky.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zewzrrup.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2weshpidb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yueywnxy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vttonmpq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhhbnnh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xwrgqbyx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvgjhpth.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilfqwyrr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2kdinfjbk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmilpao.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zyeerhsx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2flthtrak.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cctdpoiz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wjqgclet.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vjnajaln.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bysniqha.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zdgyhweg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2pkdylktl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vamfqhgj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2eqiixmne.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pqkigaib.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jzluqbzc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2muvsipgs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vmnsglnq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ugyidftw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rjmesgfp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yosvyazm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mleessyv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ngpebbec.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ivaznint.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hoovlgqf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlptnfkp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lnhofubz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wflnvsfx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qwoylodk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nxrbivcx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pweeffbn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2loofsfuf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hfpscngq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2byablygo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vwgamwha.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pmvpnxwz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kuzfzxtu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bscnspwj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scippjka.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxllyayx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2glpwsepn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qiyqexbo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ebdbodwg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2myzxyfpv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tkztinyi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dubsncac.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rhgbhhem.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rsunquti.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jgaghnik.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2iqitawal.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2igzvjexp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2embkynnx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tlmwlafp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2wvmtimoq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eaqewdwp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kcljlnoz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jtvnkkiv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqfarikj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ukcicrhn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpnoqsrv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zlikweqd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ttgtqnis.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmccburr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qkybhkdg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oohrpesb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hswwnqov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jalovhla.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sugbayzj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dcciodjx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wlzqtmrc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2irsmgavk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vlbbbwop.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqlcttq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xbgpbceu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vwwegkjn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tdufcmqk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbuofadz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mvtpupni.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lztzessk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hymmfjmk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wftjhmpj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sjzhrobd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zdehqykh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnurimi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mruiydee.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2twxmpkih.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uwezdgor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnftmyqp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kfmeoahd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oprrewkq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wdfljbet.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ymyhjted.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fapwhszp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhhhvvtr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2abmsdmmi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nnshxjnz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yrhuufex.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jpuqdsia.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzhgtbcb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwpxnlsw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rxdxfzuk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2swgoqxjr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gizbgvlj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jgscnnma.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wsblksad.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zmdeuxur.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2scrhffuk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2majoijer.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dvryeqbe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2sfxpodoy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lfgirmqy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mtwvwbnk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tqgovsrb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dsqsmzlm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dvrkndzp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sgdtfdob.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2grzzzimr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gteprlst.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hbkyrwsd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bhotrgrj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2byodvjkc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mqlhunpt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dpmqfmtu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2faiaqxld.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iorrnrsz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rvsierpj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ytkjtwew.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xzpaojcw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xaiggnoz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rljdgfez.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2djrasqvf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iazxupnb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dgmuodra.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rwesorfe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ckasozyr.html


<!-- 参考信息 -->