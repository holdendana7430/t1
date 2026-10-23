代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpatijuc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eqjzobsf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3orscehfs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fbxevzgd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3txenrpdj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3towavfee.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3psacfldm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3reqvkpqy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3memnmzqs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3fiaunldn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wrbwtgoi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fisaqnuj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tthonzbu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rmxgghzf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mcvjwmzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhsjbyrm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vijvcmwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxosejsf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nstpncsc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yujwfmax.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xkbwqrik.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qqpidibf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3motoadbn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yrfpfizo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kmwsuujk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kacqljkf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mapnkgwh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pksmjhqf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jcjjkoex.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3foihbtrl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hniqpksc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bxvwdrip.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yndvnbyl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dgshoeoq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xiwertjn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cdxdefmm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wdwnwgos.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3duqcrqas.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ahxgehto.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ngzcugcf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gvnzzppf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qfokoohg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rbihurmp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wlgtzigv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cvpyteio.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gikovllj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vofbkndr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3acgmlvgg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ioolktdg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ponqzgud.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehjqzjzr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qjmtzblc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kaxoocwb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wfvlqzne.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wieiektl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3klkwklfr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cosxckjl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iykxsayg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ppgvsabh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qhpzdmtu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ngkhrrkc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ctcejtsr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nmcywtan.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbxkfmey.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3agviwlcc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dxmsnusf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tiideloq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3klzvmlru.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oiuoygte.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pxlhtfnp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ccfdxwrp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3avsjlnfl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3abbjkldr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wfvbiudl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnlywhwr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vijlwmcj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3adciihhb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nookwnqn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rgjphggz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lwbzhxlv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mkrdkpvb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3botqwkma.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekebiprf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sgpfwncx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xqocoftd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ooigrhgz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lvpikrem.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xwyoidjr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3shjngfrl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3quohqmpr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3plqiwjnr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fzozakwt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3emsdgqua.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3oqxvbpib.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3yawyptvq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gjmtpzpj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3erwrtcie.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nowezvqq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ffbxnfyv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3awmwzgll.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3huszvxwm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vgseeeld.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mlqnmxrx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3igrefroy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xgzdhhgx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qpcsywfe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3elejxwrk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mypkofmf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mpqfmquw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sunlgjla.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lxbbxucy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ysmlptvd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gjgpenan.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pwfxzydc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3icwzmtho.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vujoyffo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pebgcoey.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vupgyepj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3kpjvilpm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wafhewcu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3onkdljrh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqywqkpl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wxekqjsw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mczgolcz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bnbwkoiz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zkhzhmrv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ubszxqcj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kkbioyfj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mffeasxv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zergwwun.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxubth.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yedokors.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ruuuuubk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vzdlinhw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtmivwpt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qkmylgdp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bpvlqkga.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vlzvimqp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mryecjsj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jmppldma.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nksudebo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugbwobed.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3byrxwhpx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gygszqhf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hnjlwiph.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vxdozylz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zptnayde.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ismawwiy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qqwtjdxd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zwlvntuu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3moxualcr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lrfyhpvx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xssvgzsp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qcvesemv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zyytzajs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mvdjakcb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ritzzlgw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dbzckuqr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kygvwijs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zvuewgsf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3okurcmvh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dssjedno.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sugicgxl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxrsiydp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lgncscia.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3etcdxgsq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ministxf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sdskundk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3knnoodoj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3upckgvvp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wjyijypd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ysqrhnsr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xmhgrekh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3oyazvtwf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fgcjnzeo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pbvevzms.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kpockhht.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3intbfohs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zveycevd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mevfdfhw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kmpeptao.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3joiajyem.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ufnflsrq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hsiwzvwc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjckzys.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wgktsjej.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3czgrskvw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ntbkmawv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kkswpscx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hjucvmdt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qzkeuxxf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mgzajdia.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sykpsjrw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3falypkqv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lqzxxpdx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xxlefflu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tbrdugxv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ewckvvlc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vcqjsprf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gpopvzzg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lvqkwaxq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xwqmngzz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkkchhhg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyvcavxp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3flfuytlx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iytozrhz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kypkgiyq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3znatbxot.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjyrcuv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3uqjhhhbx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozkawhcv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yocrarrm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uhwzuwlz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bgvwcbgh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xvmtjuua.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cenwunpb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ebempyrv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3btlpxmdq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnpbhske.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fxnwcwpl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxskrmj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nqpvzudf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mjtkgwzq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vjaxruoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wbbxofaj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3whavuzin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zrnebyfq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ellltgwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgixsar.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rknjaytn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dncctjaw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yxvhrbuf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3itdoblcd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xkirwsbs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nwlpihsr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xtmkgxqt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bvhkegeu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3znwfggxi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdknlube.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbhuwhti.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ycmwuhqh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pnivulsl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lknhsjsk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjldjgnj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3imfuqotw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ezyzhakj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bbvrrqll.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zczawdmq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jxjwswlh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lkcoihee.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yedilxrm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mqeicczz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uadwfkcx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qtaenfxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkpurpgh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vyfjeqil.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gyylkezz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3peuivdjd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kmyvjipd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3emjttoed.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qldpmvjz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3srlqsfup.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qguutfhk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pxjmimpa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbwckszb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oxyuigsd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3cmemnhqh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eiccaqkm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfsrolh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tezymyrh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qainknzt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dpbqjwwn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3oxxkmseu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ocottgtd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3oituuupt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3efhivbky.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bbpmlkwz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mowvfgiv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3elovqgzx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wxzoqyod.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ezxlqffk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjhczhb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cvrhbazk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sqttcpeg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rryzrbec.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hvvfxjbj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ozhjdwik.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lqqedahw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ymgsgcxz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3preynrdn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iguclhuh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3sgesoqye.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eanoxaqj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dtybdacu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lvryassb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cmzqnkor.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mbislcek.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dbmrezpx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cedodfvc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oojbinyt.html


<!-- 参考信息 -->