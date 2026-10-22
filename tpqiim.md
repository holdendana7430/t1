代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ypowkoms.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qyzktgen.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ebuygsln.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gngwgihf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fjdisctg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2idmuegmk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2klprpfrz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nzimvkup.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hwdmjmwr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bzzifzrs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2racxxgne.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vafopzwy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uqeqyjip.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2alphldcw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ogmayewv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pvgeagwh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbcgducp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kbnflsca.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mbtbdmja.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eegncyvy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jpqzrcki.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bmjfqgmw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vfzznghq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2sapmxusf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tmzqfktr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hktuanze.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jrzvwyav.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bhwytflm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dcftbmgp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bepzfuab.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uuectdvf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vglethuq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tstxtbhp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2gfdcxrxb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wfwvnqfb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mqlxssuh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bmfdbzms.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wfizieyq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kftjrknq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jnkwnapy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ctditway.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nevgnovo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jshblmlx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2feizuzig.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2leeqdfkv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mmzbbhob.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dfcvbrit.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zdqptauj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2thvykmmu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jkqhvrgs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lqculyxr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fbdprvmn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ixysdszc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qodinmoh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2caodefgo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zqecywoh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2csqtoltg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uncffzgl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wjwdzfiu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2obxbocer.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2psqrdrqn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ylswdcgp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sotysgxe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bxorsqii.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xtmgzdwh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mqqqcjme.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxkanmvk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jheshctd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hgdykdyz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2plzkiubc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xqmyngej.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2godlarse.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mjqihmga.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2srmmhsls.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fnotbfhp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aymcpsct.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxnbsvuh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pujuilxu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xmbfdpui.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2spcropou.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bjfsympx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbeykixz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ijsfplvm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2tvftwqwq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wiuazdoz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tgxmezhi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxbwnsuc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wfpwgdow.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gxlvtoky.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2voxabnwn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2abebzlza.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hbqficci.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgyfgfnv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wxchciai.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2drwshavb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uvfirjww.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fljzdjdj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2msyrnjup.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbixnrcu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lfbzwqzr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2erhguoca.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qtecsiei.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2irudqncn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bsldsnvo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zyodckov.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2crawvpit.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stcdpqqm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vegpdxid.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xwbzmvsu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ztxicijt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2farlelpk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2uodradwi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ogaxmnte.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pvzwkuot.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hhtexkiz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pirghabp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wsdvswsj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2btfumibk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2eatdqpgk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xwmhiush.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tsjwcrux.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lkfahehz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ethutnqq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rfyxxxes.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yupqseju.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jorgpkxv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yzqdmcwf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kotldbin.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlogmext.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2drgmvktb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2piswpbjb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2riioqvpe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2aqlghzdg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2laxpijwg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vcwgpimj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ncpcddgk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lesqtinw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yilwnptc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qtletumh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kltzcmkf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2daaxheur.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ndapdrud.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2usigbvxy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nfvjjdxt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2begstmch.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eloqomtf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2meffhdvl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gphzkolv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mkcemuty.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tdusmyrm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bvrciwdc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2llbegfso.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2elndqkjz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfqamtlj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmpsktpn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsfrdsfq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fhorahbz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afxeqdje.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrohlblz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ztvinvee.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrlanxhu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uujvktrm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hyyzqxyx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pmoyxmkc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rbnxguit.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gxatosib.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tdducxbx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xjcpptqb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2blfavubh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gnekdvpj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2eflrqlll.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbuuzmo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vusgrdpr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2uzlbfwbk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ifsnhugq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bffioyoz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zpzooork.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2apgzwspj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ptlayocn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ctclsnnx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxkqclrc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yqrieohf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ghvybvma.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2elceylxf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dznqhikc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jphwttvu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2owryrtwh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ubcllogs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ouurliky.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hevedfsg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpamusaa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsjwklv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mpbjtcbl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rezsejpy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrqqzuc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dnxdmgow.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ofdgocvb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glntdbws.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2seierdlj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nwyonwqe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2upygpbgm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ezpfwcix.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2orkigokn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yxxdalkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbkcgkbd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dxhhswol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgruamkg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vfjpxrcf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fpitajiy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jwnbgobu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ktdqrbsi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tdqrixrc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2awzbsban.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhxmycyo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2btlbbpqg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2petngfym.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ioadddcc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zyvcznes.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dqkrcdcr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qlaulokn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gmxskeyz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2peigxztp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2klmveftv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iviplevo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nuzwauxe.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cyxcoplw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xrpdqtim.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yidnkhol.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bgsfencf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2stusxwvc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2spmxfrbz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cyepyjlb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2byauqlae.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2utlochig.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yqkgbbpb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nammntom.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lceuqruk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uaeicdoo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mltyohxp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nykjuvsg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kjegbrdf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pebrdgeq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pzokewyb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2akhrwmgd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2occxabna.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bxalqrgb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2speathmo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2apexkkvo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ibeavvtm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xaxqchoo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fbdvmeoc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2suxmzvpq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qgzpqeli.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqglzqqs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fbakmelc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2moaeyluf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hialtedg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ekgnlixs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzirdwwk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzxbguub.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qldchflu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ridhknro.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tugxneeu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ufwperbe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jmbouxcl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hluwninl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vmavyxck.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqypbiwx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qctgpdwc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wtakbitk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xpkngbwd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lremgpcz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2krrqegzp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gnklgndh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2spxalddy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2glieciam.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2uozuqsag.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kwrkhtzc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dosucnpi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tnmcbagc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dmhyrcci.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bnjkratr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mqxoojeh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hggjxzmv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ntyceuqu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zngnrfie.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qepzuqam.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cdsbpfau.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yiizyszk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2alzerhqa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jutxafga.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zifoggrk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fvokvklk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ztydnshu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lajlnagq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jqfbjeok.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uuhgqxso.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vfbujolu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ujmsfnrm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2djisroys.html


<!-- 参考信息 -->