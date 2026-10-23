代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oprlyeuq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tgsiuqmf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jymfkwmk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qhzbjnsk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ljlrpern.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qnbjegrc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uirmxuez.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ghusmbzj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3krqvsnhd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eqskedww.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qxitskwl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vyfwhnya.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3phmbhlqf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xpvkfsio.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tueuwwxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgvpphsp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hajjpfow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xphvdrqa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vdaryzoy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3aviasxuh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aoetpjfw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jwwsqvzo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bbrvmxre.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lpjbnkvi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tldrjofr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fbrudhzy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fpquunfu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lzdgwwbb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3nxivckeu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3czzgdwdc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qipubtdb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wschkthq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ikclunmc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jlqacjke.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3llqxgntz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gyeupnmk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3aetfygwm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eeejqoxc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3baewkjfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3iirrzhsi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uvqmmuyq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3peayljlt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lisxaumk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmycflq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vfatkmuw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kykwjumq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zsngvvxb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3agitqnrx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xyevvqht.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yahlzegi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3askxgtqe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kblvenob.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lsnfkiqp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3evndoowk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bnlkfhyu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xvkrsuek.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zuthftvk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ieruwsab.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qhxgvajb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vkfuiymd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qxokcgsq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dkhgdgui.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fujtdmbg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vjzcjwoy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lywjncaj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mevoment.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ycgztfnn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3inrnhroi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3erfcmvmu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azebwfne.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pmgrpcbs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sbqslegh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nfukvxmn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gsmdtelg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mrkruxlw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hhgthsot.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zxexomol.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mardfzew.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3acqqinvf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tlgcswoo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3thlplska.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xqgfwqdu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3trzfgozy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3delgexir.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3phowxgvq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rgijwghw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmwgdiba.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qavrbwfs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3njrxltvh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxuybjxw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3giqgbzoe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cakonatb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3adajbgjs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3sxislxqu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3owpafscn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3sqetcrra.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qnrmeilk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gfqlvops.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cfqgghwn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qxtnbtye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3apnuttya.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gfkuyeps.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dxdzzcnn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vjadqhwf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tkioohhv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bvxudyex.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wjjkymkz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pmhgzlfx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3eikckeyh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pcrscdli.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ztikrcds.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hdmzcsqc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bkisxwyi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lgvfhnia.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esuknddl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fdhesvfu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tpctyobh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ersftknc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gzdmbrle.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3armcrcio.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3abngtgbf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3henozfqb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gmwtxasy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkazbuok.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3isiccrpr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3huyspors.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kgelhbuz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3imsejekh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3evkomyqa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vbrjizsf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3psulwgme.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftfwpjgl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vydlekub.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lpvgltrr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tcvhnbeg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3uonnugkh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3returunr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dszvmsad.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fpcmnpjo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tnpgrcwv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aareddce.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3njhguhcc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xtqhmvwd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnnyxjar.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qgjoxkak.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zdqrdpbk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lehcvngb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tzffwxsz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vjmdpdcf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uazvpanh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bfvsbcvq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3aenbzgoi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ympngiis.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nspuznom.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3deihypqi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yfkqxgqk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3upmorbce.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ciezqaew.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3axvjcejr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ryjgphwz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3elofkwoe.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3iubznijv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cltghlif.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmahgzxg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxvvnibk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwfukkvw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3oawfjgmb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vyudeiwu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wfaihxkk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vssrirpy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oqmgivyx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3edrueote.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dncvtnnq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cresddmq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oqnfkbhu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zpvyzneq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hupifcql.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ewnyprwv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3thbxvygz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lmouvtam.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmermgeq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wupkkamm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dyaeywjy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rvfwrimg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ozyrwjpy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wnrnywdc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ekbgsvof.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3uwvvpqzc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xbooqltb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pnpkmcnx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3alifactp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3heitvtjn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ircotabh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hgdmhveq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zrxliqfs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3sylsqnvc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3bjoynyqk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bnrnykay.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xhxianks.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mypnixvv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3htnfzrra.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3snfusfmy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlmdqgyr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eahrkvoh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rsodajoz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyldvxsy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xetwbbup.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fsythnie.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3daysrygq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ngetmlht.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvfsfrtf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rlioglzy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3usbheshg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hqkhddhj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ivmmpgxt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vptdtndj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3brbsxuwz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfshkgkg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rnrsdhxm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcoplzf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hlxbierx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aosvgbuy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltrwneox.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jksbjxzw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lgrzjvsd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3faqvkdtl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ggsswizh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gliaatlu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wwffbqdl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qdlvfguu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fqiffpdm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qtkoqrvx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3spcfrgfy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3eiqkjnlo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mowqjbaa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qklsspne.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3djxgshup.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vwkfnzjt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gsgeghfo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebkwvpan.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gegpdaty.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nqppbgws.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkpaqytf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rbjqzwlw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3golgwfzu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdwyfvja.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kubojhsf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vrighmcj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wjuwzbtv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3llrxbqfi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3twxbmqts.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yawczkfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmhotdqv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kthyijqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imepaxru.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sesioeei.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dgkiirrw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rekoidgs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jsynaazx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3svbdlzij.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cgnpwwbd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ibvlsfeb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xqqxcxbn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fmeotreh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3otuyfuhj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3utrmthyl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fcawkrmo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zenfsbgw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eankuwvq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mrbxrrdj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xurzpdku.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fqpywzeh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cijkrkwg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mkrbxsfi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wyxrxecd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tqrsqnsz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcvuwqc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kewiespy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uicxtjyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yyiqkykm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3viectazu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3swlutlmj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yjuvdiks.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rlxzuhhz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jqwuxydg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqsyhmwl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pftrxokq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nxdtwchx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3adwyjqax.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gmhbvyuo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwynoqgz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wgnlcrbh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kqygajgs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hfirzpye.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fjobczpc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sazkslmm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3auooutwr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rhnccnuo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qglxnqko.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ntknrykt.html


<!-- 参考信息 -->