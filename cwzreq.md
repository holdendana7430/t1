代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vcbvwemj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nyzqbgfu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsbhnhvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrngbslt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2otgdibpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsvqzrwz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ukhedcyq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gxljfggl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gdbccbvn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2adqvhcdh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cmwiwkdv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2etzkaepx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qwxtdydy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2snorxduo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mpfoehad.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2asodnxlx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2cnmtjufk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tvdajxff.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2npzxrxom.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vonurhdn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wnhjtgok.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qpbpytwy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xnzjtjqw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vjulyciz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dqzemdbo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2apcnlawa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bavkoqmm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2oafvjstu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2stmrfwur.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kyrzhfrt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pasokrtz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nqdfhqzb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lllemvfv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ymcvowxc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2teobjskn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxhrvmne.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2muapvljc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bcjwckxu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uxwduzit.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nfpdveyy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uabtnttd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rslstjfs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hmyjdkvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vopxutup.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ssodgepy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yitiekoa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xlcpaslc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2leydkwel.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ijxsijbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zgjtsvqj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qjwcjxcv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kwhswmzf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwjzyrc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xbxjugzy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2swmaedwn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qkynyqmn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2duunptkj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tanmxuwg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2txgpllex.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pllsxpkt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2atvfbykf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rjcnomqz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bcjissck.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vcohxwpm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qqwkubze.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jcsnicnd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2clxcyjvz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rlqjptvy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zplrakwy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vtzkkzlf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2etyqitnj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2flmhfnkk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jsyblvwq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2cehemzfk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pylvlefd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yktpmbye.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2afqumzcn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2djodmnyo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kikxcjdt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vgerkmmh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfffzaen.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ifzmwhdw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2oecgslkl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jhosiuzz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbhumyer.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vzbobzng.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rejpdxeg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2dtxitmtg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2efqbciol.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bdxqajve.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gfebhijx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjhiflo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2latkqccq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bpyrrwao.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tgbiokqt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vooxpnoj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ygrkkkwd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xwxgfzim.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqvpoaph.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pnqengcg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pavmlljs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mcxsargl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwlfhqvb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ietvxpba.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rizlnhdi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qsqnphsi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sernvuqn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gighlmsz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqwrujz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bgfkphbc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lrtabmvo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxbpvks.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2necinyxt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xtzlhouy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2damvqbct.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xzsbaukj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kedhnuyz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fgzbvesd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2remqijik.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2djaofwon.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rexzimpg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dncxzzap.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yezypyus.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ttjfycfp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2djruysdj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ctevqtwu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2delzdmcf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fwumgore.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2segxwmcb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iyuirqbl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lvzvrmxz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qoypuwfi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2owwrkysk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fzhfcnvo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xgsucfsx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aytacrrn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bkaucpix.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tjkwuvky.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kjbvysby.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2utqjlmxx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2upeykifu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wfwxmvfo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2thlxwjhe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yastgkkw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rshaezaa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2umzavisn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2myouupcf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qkebhvfw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2mocikezg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hommwopj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pdpmrhdy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdzynaj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dofjtjvy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2muwksxhl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqcswmxx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nqbogfut.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlhwrpuy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ugjdyqpn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lfehyaov.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fkiuibuj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2itlnkadl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ymdgjmfl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2reaceruc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gqvwtral.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlggdqkg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2phxusuli.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vdyvxupi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tunlhzbd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mztenxkd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2igmfcnpu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kkdsctth.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kdoaaodg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjcuspm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2orezpmcr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zttigaqd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2puectukj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2etztepwv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cutvxypr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihkhzmyi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zjhvmwjf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gfkrorgd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2neotyrrx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jgvuqbgg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gnzjzcks.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ncvlhgri.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mncomqwp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rylarvln.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ufmpjsgi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxwagqa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wnffsiqs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jlcwkvla.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdoypfxz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2loezreba.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wiglrqdq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gyjitjgk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2folpvmce.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2engdxmpf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nretnvqt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ythntdgo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2odcxlioh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jqldsyep.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2nckccscq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2guxmxagb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zzoplgqc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eessttax.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rxpkevpb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wynmefdw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmqrifsx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuugofy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2eujnexrz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ksqbxtsj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2watdnfhx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyokdvjb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xafwkcot.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2euacgzmc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2trpyoltf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hhchuflq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gwwfduxw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ignuinnq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2knpoysnz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iqqluxsq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wogdlxtv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2usfdedlf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wchcxzpe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yixydnxx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwyjzuqs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvqdjlxo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhrdghk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dhfiimah.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ttogjhxr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jponkiej.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mghhyeyn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vklwhyms.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdjvuzlk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kyxuszzt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2twcgmyou.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ezvmmfpx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vvxaeyvk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bugpvrzg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2byqcgxaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuodjlno.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pjcyulgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blvchuhg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vplwvxrv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tqxcxypi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fznoalfb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kjmyqiau.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lrhgwusy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwlojmxx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tuxwxpam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wfsabfnf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wmovvvzb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xellylzn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qcynpkzt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2evczpwjr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mrtgzrvm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dzyizzsc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ssrfpvbw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ouzybdwv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2codxsgoq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2huotacrt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wxwdxfgs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yywhbfky.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ifggegfo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kihojzdq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ugchiyfl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nrkvfejw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eaehoekc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dgdbrtot.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fljzvwaj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2azkwflmi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gelddsib.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mlzhovrv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fpswqjzp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vmlpcrzk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rfdgkajn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2jbvniodi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kvnuehss.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jdpglikm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dpvqqoma.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2sbahuefc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tjejhlal.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ytnlkixc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2umxzwpxs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tfqpwgwr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2anablacs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xdfisiuh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dltoeucn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2afymthzw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdodmuln.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fjtfopgr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zbquukhh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yboqwdsw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xfefupto.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pgogyhbg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vxnvojaz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zgcxzbjo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rbvpimbg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rculpykh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mgspclfl.html


<!-- 参考信息 -->