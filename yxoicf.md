代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rnbpghzh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2efiofnnn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2afdrloce.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cnqtdsvf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mjqypxcf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ocrlfzzd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fknzkroc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jukrrmwz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mavvgzih.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wncefghh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvqrvcnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hocthmkx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ffcrziea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvrjrrfs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2alplwwvz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fgoipzgl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gyezsypr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tplmcvhy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ajzhntsn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2blxtlluj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zijasvcl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wsfpjfnz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cgpuylqg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2oldvptfu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2cwtpstwr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2foxntpgk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qnuxmylj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ksdemnyv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oxwqpoym.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dozhcrcj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qpqskfke.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lqrrlclo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2prsykihx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2clnixkfw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zlvahdtj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hjrpmvjg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jsqlsauc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gdolepvr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bhvcjiig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lxuloqqx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dxsxivne.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tdnchehz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xstlcuaj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2osrvnzgn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qukqltky.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jwletbey.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eohhmbcv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qwflffhk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2woaogepg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gemvmedp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2pudaluio.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eskbimki.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vcdrquya.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2axjultcr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dtgikgyv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2grjjdutx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mkbgkijn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ceboahrj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fkptmxxw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bmntulrf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jayvlohp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbxzispk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cpvrspxy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2csnvhmiw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2boizkznt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hvbywbgr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kirxyuxi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gjyojafd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zkmxgqgj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yudmngqm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2varrwgcc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mhtkaeok.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uvioehmu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dpqvjdre.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rjvpnwwt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2izngqonc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkcpocxn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2eeagnjmc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jyvceidx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ktgbjsnm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rlozflpy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ggqprtgy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lyswxyec.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mpjwumrj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pmipseup.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sifehktq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2inrqjvat.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qdbcufrp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lgqvdwjy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lgrirmrm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2kimtxcis.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2sbycbubo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvygbwsj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hdgdlogk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lzrdmmig.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hucnyyfp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uagtphvk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lptvbffs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lnapibrv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2irtuhcgl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qaobsnus.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uhsvcimn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2eirrtjzh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qpqivonh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lclwjayl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ddmowfcz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wjpylvcx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2trdjxztb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hfxntumq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fjxngxab.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dagrjnkk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hksbpphd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uivenmyx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hfsksdgc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rvftsoxh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2egqpvvkq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxdanfkn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2incekpap.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cdxopkuq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lainsaza.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubidbnas.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ifqbsjvt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2alkkyvwv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eyhyhzho.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jkdykghf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xixojkyu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fankhjvw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rgxweell.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qzvdujji.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qeqksmjf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xiaklguw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2odxdjzwm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fsfmkqlj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kdtxawpb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjppfiur.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yezhkecp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2heitgefg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bzrpuuxe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zvtknjyd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mtapuyqg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pszseimg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mhujpkuq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ippglbte.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fctstqtg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dlztuqjt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dwwoedbt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bkjmlyry.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jgawleqc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmecbayc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nyminqdd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjatsgct.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bneyujbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jkkzjdeq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqydewz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vkfoqluq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bwngzipr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uydcnxas.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2retpsvej.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pyxvltve.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmerhoxv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uibfmuzo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fxlzjthz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2sdjqodnq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gqgjorlf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gungktda.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2owxypxna.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2stnywulm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gcexcocp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ovajlyzl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bkhhcjif.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xnuoyilg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2btnafwnb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hqopminu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sdqbsmae.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ezbqzivf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbjjjtne.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yhxtbswe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vldrcdaz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cdbshqun.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lnnewitp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zivcveui.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lphasgmq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fceckidq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2uucxxkfg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2geidyyno.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jtgjpbyo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dyciqbgt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pwtzrtvt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2efjpujbg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nnnjnyvx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hhzblsww.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qtigjohf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2grxpyxhr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dmoyovmo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vkjpejon.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kfwgckle.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kckznhbv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oeahztny.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knirmfwn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjryvfd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oijxnmfo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cawsdzfm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zggkawyi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2umcjkijf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iyxxocqf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dxqisuhb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgqizgg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xgspxvgs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2llactvvz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ymnsgfzw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lhwkgkub.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gzmfxxrd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jhhsixzu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wzthqzam.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pnzziayt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2heksjxkp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bbfrsrzw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mgftzwyd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojvdjdia.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2cvxfnsgh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2sptflrwc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vcgctfxo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ugwymuiv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fcydfoty.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eiydsiph.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zztkxiep.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xbimxrwm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2syvpjebd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rrndnzzu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mkoroqwc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2sguhsitu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vcqxnnvq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yuugqomo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnssjgaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2aqsxjmom.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qnndvusc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2atssvfqb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvisksj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nczdfdlh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ieskxetd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bqstxkdz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xczgcyao.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ihcyydpd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tcnestud.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tasyyyez.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2atimbxpo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tduafypn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fhdobbju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twnqzwln.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qiobvtmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpjmlwqa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fvyxxsvv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2trdhnkpa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rthhlfhc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tdllvshp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qfztfcbf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zbcnoosr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxxfjwkk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mgegjrnv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zopiicbe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vhxnsuji.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mlejhotm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ylihnobf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pouyoqbd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bpyrqpmp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2djybhcyc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzlexnyk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rlnldqho.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vjgtdkrl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cvhaotnd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ucaplnld.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zratmokb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kqnzlvjk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdcpcbo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nsbmvubk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hxkxjqbs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pcgoxzyt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xntbiwtg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hlxnzrjp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2acurdygj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cpnffyux.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iekcfgbl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uqwdzaov.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aesxtwzd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cblbpogh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgmysrtu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cnpfsthh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pxduwbby.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cslluruy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2avjpuspp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmziybil.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rmlqfitc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2niavstjh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2edhfgzym.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ikzuzacu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tnndmtis.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2itgvzcii.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iecyctok.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2epztqlen.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2esjvatgl.html


<!-- 参考信息 -->