代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hsztnupf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vhcxgsyp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wiktgpif.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vgodmihe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3spctwirw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zzzxfnxv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gtptitix.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdgbhjfl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bwzowxlk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fixtxjet.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbrlqine.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecgjqnnd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3reexqipm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxoxjcjq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dmfwfsbd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ioyolsra.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mdxozaig.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mpuuidqc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jsafzqrz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vxvpetef.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gawjudvk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zexguzec.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3bnjsssne.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3oisuiixh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zilsvugm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vuqrxyjk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3baxipubo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ishlyqfx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3usaujubt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3awywxngb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ghnhrzox.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cgcbugsh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ikqvjngz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxdxfew.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bmktpmsd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vbfwbaqq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3plwldeej.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tcilnewj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3duwmylwy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yqzuvxdn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwjzanpz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3apjnbvuv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3tujaushs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nyjsznmo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zgocpqhi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ivpqezup.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3emtufxmb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xfsxllfq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zcwknvzo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nksggdtc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vcredman.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eabuhqui.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tgidslya.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mgqqmtil.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3zuuefmvo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ypztcwxu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xqbdlewo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mkrttapa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tqnarvnw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3izjctdqe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrbydag.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vlxmsgrz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mfeiycps.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3edqwhaqp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dyljhjtu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kzhzxlyx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zvkqyrli.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ulyjpxsu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qmsnyiyt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qdruhvuv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fnsyrwzo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucymxmyi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xukbakju.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wvpfzkqb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3khaavolo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wdiwchqc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gufsbtod.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ikxqkaox.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bsbjgpii.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uuwgrtuz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3drgqzdgy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vqapiitt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzimkfqk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bhjirfgh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cvzmshxf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfozbphr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rfifdvuz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3abhlyesz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3brjarmdr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3fvdghvhg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3pfliibpx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pgbpmudz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqriyfak.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gincjvac.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gloeczmb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qmehecst.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xquwldqw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqqweglq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3awzymyaz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wznbztir.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qangujeu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vouzpyrc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3neqaolrd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3miyqmcrk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mopczglm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3giavcnii.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3reeujbce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3gghyspmv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bgngvpdi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dgbypisy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brltsmar.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fbqukmxn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ilmujpua.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3chssuucn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cclkonha.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyzkfbqm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jxmcencp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3clyrmmat.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3aagaosqp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pkvsmjpk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuccmqgn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3felhvrlb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vojhbgkd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3szmfxhth.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hdyqeauv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlhxnef.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iupurjpq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ikyxwqdw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kiakbrax.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zngtdnoh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwyjwjlj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pgktxlja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gujhwtzt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ioaxztxy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qntiujpt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bssvfela.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3jqbfjrkl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nqihtcjz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xewlsdci.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3buqdlkde.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cemsolvx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ezpmcykj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kzstpxzk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3olscysin.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pscoyiti.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3khzefdod.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ulxechpp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wmrexqpl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3skdhgibd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gtalrzwo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhwciknv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3izujtjun.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xgpmxthg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wlfjbzzb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3suievspc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dkutzfyw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pspwwody.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wkpmaplv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ofonyglq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oznlnudj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hzsptnkc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3krojrtqk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfkfwxfd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3utgnaior.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3seqaydms.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qldzxxxb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wlmndscg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ftzzgbsa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ckdoecba.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pzfjcrji.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3eyiuyahc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jumrxzce.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3aigvyxiy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wqznvzcp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mmxkmqcs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yoxiygqi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3iircqozz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbybphwd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qavpgapc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qqdbrztc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ighzpnhf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3aulkhbti.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aiyvnhwm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bdaoripx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3grroqplg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3emmqvinc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qxuarnak.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jrjzqbsp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ukdmuknt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3menxofjw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zhjdenjw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tazwhbjz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3spfgtces.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xpwunprx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fsdlolpa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qpbbtlmp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rdntzxje.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eviziivg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hrevcapr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbpvnqtg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ajgqvcas.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dompymne.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pbrswdok.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hcakrqgw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3isgegfgc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ynvlhfjk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlskguiq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3cekmyoam.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dqwjbles.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fksxggnb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3iupuixaz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ephdquzg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fjwmsbfb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xohkxhkl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3olywvigm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3klcbcaej.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wodlorrd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rvlolkcv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3afzelpcq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ntzttlmm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3orlhknax.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sftjytke.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jgpmbqgn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kitgrule.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcemmgtr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3apcakbvq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uncvczfv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3mjnkexec.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pttjauhf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zqhfrruk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tonrdatz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3oujvbowl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xldomjpv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxhgiug.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cnuprlsx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikjfwvcj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vokcoxfh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tzkdzuio.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfaxais.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umlckmod.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dgruhejw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ziigfbxl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cdnmcexh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tecmhzok.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jklswhhw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zhblnnht.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3odesmdfl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3suakfafy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgndhlyh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uiwwkgkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnxkvbkk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iyetzzdp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pinipyvi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lkrdrqnj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wyiivkcr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dthlkgxl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vhfsbvge.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wchsnmce.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ikomzzmj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wictiqnd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddmimeba.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ztewxtuk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pgxkqwrh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdbilmc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ifijnpny.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3osanzzrh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3godfdbhz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wmjfybpf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gfzpmhos.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ogfhcwmn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zgdvsayb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zqywjjpc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3apdobkgc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nvkcoxal.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zaapcipc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tvefinqp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3prjtbjsi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3idbrytyq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eusuwaqy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oofrmvmk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vvoydmee.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ooiwfvpy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3koofwmpz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dqgqobly.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jgbmvqyc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cahtszaz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3naiqutiw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kbxwknke.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iutvlmix.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3inppexsb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jlzvbskc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mvttltcc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ucwbimrf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pksvksaz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rliizyuu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3efxyuhme.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ccfjlvzt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygfyvjxn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmdjgnar.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bphvaeey.html


<!-- 参考信息 -->