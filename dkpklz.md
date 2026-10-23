代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cocmgtvo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wshusmcs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3uspkpvyv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hhyeptlu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jjztbblu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wzrmkpbm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hlipsnzf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ynbyhubp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bqavzsgv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bqrzeooz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3almbdtil.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qrssutlc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lndsybuh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ngpifrks.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qdfhupmp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wwgewwpq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpazvqip.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iovswonf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3iijbggly.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fzmczhlw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kqpngcnv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uafnmmjb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ucspasow.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3utswnmsm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tazpzahx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ngcvasws.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dflsjmtg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hnzsyttg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvcvtuyq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3majlncsl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3enlkkbop.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ovvgavwa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mxayxwwl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mutbijou.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqhhnma.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xtohonuc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3klybvznf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3obhmlgil.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3edmowmpa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qmikrvko.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ignsycji.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ugsuuaeb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3potpmcec.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cgfpakvv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mggpoitv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yvaxqxcw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ncjerahp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pcybcytf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpfgdamq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zapxwwwl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fipmzjds.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3brfaxnnc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfhlar.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3unnjyzaa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bfkkfhwl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cgrnvczg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pypkygpk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jmwsiwrj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ykdvanqj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hjbinqsd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ukcfanpr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3frbdfdba.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iqqasozb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ujmonmps.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vjxickwm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3trgybnlm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmfauze.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qinyflrh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rilmomgt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iigrvtpv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dabheqbb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yugklttx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aezwsxwi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zjjwarao.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vuzyoceu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jenppgor.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3koktmrpj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gphfimpt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zvjhkmjp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rygclntf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tndpyzdh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rgnrbtzj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnnjouz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orjcjucb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3sbxcyfjl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lcedugam.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fyondoyg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cwocknle.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fmpkzfma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ipvutivd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3adhrmxys.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kylmcwle.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ssxzypxu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3syhvxsbw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bjskltxk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvuedfyp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wmnuuwia.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3apftdpgr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rrpvjqbg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pvprtmop.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fghvjozy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3biehcjsi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vogadsjq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nrzsftir.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uswgwyyv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3abmaulvv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdgkjbsb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qkmavtcu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ebexrcmu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrnmkhvh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jmilejtk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ihealcmw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bvnyoktg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jvtwlsji.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ykprfxpu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crlllufx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3icamjcoi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3koqqmbdy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ednibwhu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3okctjvgj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ujdtwbir.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dgbpkcku.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3asqlqdqb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jgzpiala.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rdedpxdk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3upiwheuo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3smkzfdxa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sthvlmww.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plkgobja.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jrhqklpe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qbtzxnoz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yhrhoret.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qwzjthna.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nrrreacr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gbhxrjyx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qlnmsors.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uixrledd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3higcrqjb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kotjxypb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qjrripvb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rkkyrffs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jmzyffqk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ozydwwlr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wvcqmpgd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qddmmeti.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dzxnakdw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mbzmvtwe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3okvkdetu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hphgnidy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ssnesfkd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pddbvsbo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3inhhaalo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nvxxnnrx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lnctvijw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3drdmifaf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3obzzpxrp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wpmprsft.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tvfofqvl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vkbcvspq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vrwxdymr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qxjznadj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3galnchsk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blvrpbud.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3loiydpoy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tetynpwx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3leuveygt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nhwasmkw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lldghgvz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fdmzlycx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yuifnrqa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uxtmcfqb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3klcaghwi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btxilpxf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ksogaijz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ozlpvwvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fsvlvshb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3meainwam.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3woiqbogb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jvoxhjqy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jxugpbbd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3twhrpfgw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bcdajqsm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3grcqpodx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gpwiymhf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vpreqcso.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nmootwws.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mxgybuba.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fcwfroxc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pgnkszyv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3amzyneka.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pduadxlo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3didjmfmf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ubxnuion.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3szoehplv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xeliqxjr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3owvvigho.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3cgbggixd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ngbnbixi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tlkcmutc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bdnanpdk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bzkmhjgx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fslqjamx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ayyjxbse.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bozvmqlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aezlegag.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fcivtnqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtnlbtsy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dulugiyg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mcvawrsw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahiflunm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dpughatg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ceywheqe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yfckghct.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lpfbvder.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yrcljuft.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kiouezbr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hpjgecxp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uldyjwqv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwfmahag.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ibjfhdtg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xdnasqjx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ucvltfzf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lnktzsus.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3incezgob.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kqdccbuv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3olhjjpdk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zzdjhzzr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jaytmefr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cgrocckd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xtnlyjsb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3esaommpx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qvhagzom.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3szrnznnu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcgxgxjp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ejtbhkbk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3autmvopf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dqashggi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zogawxmp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fceeijun.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kukvjjiy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ssqrhybt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3czopnaxa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wthinppy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hawfrozm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3blwtucnu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wdffrrpd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wlbxuabz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xrzzycpf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eaklhndf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gudhyoex.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gfakbbtt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nokqtkuc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tvkhgici.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3apqzxheg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3whxwhswe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ogweduto.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jldxkzaf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3njcwulou.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzmlrmj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mhiyubld.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gyyjmcqx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bvvonhqw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wtgovyvi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vkenzufj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjcubup.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3plsakeuz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nirrshwa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtpurtw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3laqpshok.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yydmivtr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nzjtiyui.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pgrweowt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3shyzkclw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bxbnegfs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3farkispk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3clrsrols.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hnzzsaah.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xscejpia.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgdnkth.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wpxltznv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyjdpkvy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lzpahgvd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dbpozboc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3legqptxa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3moxonefc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ulzberyo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3omcfezqt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jmptsbyd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3rrnadibv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xwqimyza.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ynouzaut.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ktjrpeos.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpaqmqmc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3knvemedh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yblsimiv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xhdyhujl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zeixvrya.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3omjjwsze.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lnnkpezm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tilpelem.html


<!-- 参考信息 -->