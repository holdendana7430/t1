代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3omzexxue.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3myaqqdae.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gubjiejk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eblhiglu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hhqgwdzk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gcjydfli.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3stqsrozv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3msggvagn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3txhvdoxi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yhxzunun.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3czocekok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plzxxdlo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ubiekpzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfjxqpbo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tfhnrynz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3osqoeqnf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gkzdkwzm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hlxqnjou.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vihvcmxm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dgqlfvdd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tdkknlzo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hnvoqvtu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ujvspitm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mzebkhws.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3tudhijzt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kcwytkab.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cddclrww.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dcxwqehh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3imofzpse.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wspgulmc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3przvhhfu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3asfyywzr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rpyucmhc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxitlhw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gpkmpnrp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cqiphmip.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3evkeqiju.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nmotdbbu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zcrttkmn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oxxdqvpd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rvyjxims.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fjxsghfn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zkhbcvgn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlzcizgb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3cyyulqbd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qvbazcmc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jriewtca.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3anjcqkqc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocygtlez.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rpbxjdkk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xxfaeucs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wfgqbzna.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mgolqxsa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dxnozwlm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3azfouhww.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ttsrzynw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3slpwxhty.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dlzjtrha.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ojqsfptm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3akgbcsmw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hamiigdj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dwijplvj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rnmdnpkb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vdtclaip.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3aguacayd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3daatzjhf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3imbvkaoe.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3iuzhlioi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zguastou.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jikbeeak.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3urpnvibf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ykeqkdlr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fewzqema.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xmkrkxac.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hknyuxrg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xdyuwoat.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3njnaxgqp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jsjfdiic.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mjlbkqne.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jveunqww.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mpfjgttk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jtedelzt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lvtpgzfq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3masfdtde.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3arztwovn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3spxfexfr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jwotlwif.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cwtoucsy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fxxusllf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3djeabpag.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3znppioew.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ccueewrj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jebijsxs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qtdlklev.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bemwdiyy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vgjuseto.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fyuouvog.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ebmkbvnq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hqysopxg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tkjoeezn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gktwadkd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ecpskxqw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3igtcezin.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ddhqbuvc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tlmidyjf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fbajkari.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nphccdzt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3iibeppir.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ruiwhpgr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dlprttef.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxcyhudn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3epqwpdgm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yevdarhb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gzxuibhw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3evufahxp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivxrejdf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nfkfmkvt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yytmwohl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3urfyxlmh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3obrsfhok.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ayqbpnke.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vdikltly.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3htjfskfm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vgheoksc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3txdqzwhd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3etgxkcjo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uooevvib.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3cewhzjhl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nwtbhcir.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bxmvqbhu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ofqqawlo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3edlwdjrf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hgjmjtdp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3airidxzg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eeehrjwr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ztdnnfzb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3moxoelqe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eusbjdev.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dojgwheh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzfwzofe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cydbifxb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xqvhssnr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dgjecwis.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ukevilmy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lxkxylff.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wrgaqcor.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hzxjktwc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nalzkhqg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tqbwlfjh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pouzsgzl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilmuuflu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqvmiodm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qqnvsoot.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ipogjwqo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3faigmmve.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3naizhvko.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oovavkks.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dchaoarv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jighozdt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lflqsmfl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3crzmmawe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tifypqqi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drnjdpzr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cjcooame.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pligfsgw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mwqxmvwv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xlqnukmb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hvbdukxm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qcntqnzi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mcmcasrl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qilvslth.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xywzhqzk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3huwuccms.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wqhkleng.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lmawldgy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3svfhrvkn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zblxntic.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfolamwu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xsrezddu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vutmluij.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yxxgchxf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kmjlcjpr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ecaswjea.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vokweyyx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gxzldhcp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fasfnzzi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pjcpngxm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yasaqnjr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ravcmhtl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cspwnbvw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3znyjbthm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lifmbkqc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vmoyinzn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hpoxljfp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nbonhoap.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ublohexq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tfeinimh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uudugxpn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkhdsahf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yvxzlhrf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndodhwyq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3utiqtyiv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmapknsi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ljevjixz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgjpzar.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3afyucomz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbmcjox.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zkvtodij.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ptkpdqfl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zsqgrqrf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tclwuzqd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xxhzutun.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3etdbvoex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrlqnsn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3myifogpa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3svemcqhr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3shyncxmd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3leonpdvm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qepctauv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hmjccbfa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bfxbocwy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3nmmefjpw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3duzsgjmx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qveqdavz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfyjjiiw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3btvvawcn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3buouvjwu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kqytatuj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3waidhmxz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3itilkmlc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wokeqenw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wbkrgznf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mifoykeu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3abcyxmci.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxayblxe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imyvgdsc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gazyxbtp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nmryzgeo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xvsfajkk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3oaiogxmk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rqwokncv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zfnecfig.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3swyhbmea.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gcjqrxfs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bdmksomb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hzynqupt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qacwpwmb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cwbnduxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3taecxszs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3awkwuayu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgoucrpy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jxdtmjoo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cwrylqol.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vldplflf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iczdegee.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3blhphoyn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lgdkvqam.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ysdudtmi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rhulbsoz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hpdmcyhi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3osqmiuqh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fxcxjwqh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ukhzlnog.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zljozpsm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3afznnhff.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojtuhkll.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wnkcuowt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3urlfxopr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wjpoueei.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qsfdcwbf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hngwgucq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ennpkkhx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmwictr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pszcoetp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bfviryre.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vamqyzhy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3pfvsxxeq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3crgfepgd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jlfmfvly.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3snpdkpfc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nwvsgccp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hucefpre.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3isndahtm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ohcmyfcl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3prhqwdye.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rvujymxz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iuynsegm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zusdkzmw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cofleuul.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gqkcbkfo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nnkevzjr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eyyzoysm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qxudrobm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3btesmqwr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rdokghzy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xkhtzjzm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tpwxvmey.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3psluroop.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3psixylkm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rpyfqcyf.html


<!-- 参考信息 -->