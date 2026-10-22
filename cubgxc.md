代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vbilcpou.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypomdylv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhborpnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igatorym.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2durfrfba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qamlvjxq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cwsatxgs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pmhnxurs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kmzftsai.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aoaicyii.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2eewzosvh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qvaqlzbq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2oiqqnjcl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dgquwabz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zbtedwbm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ahfpsmyg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2affxafiw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2adbupctl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zvderequ.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tdqdkzqe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pjyveixa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbcymit.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ebrphuhh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uvnguhnb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2abqrjgyz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ihawzegq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2puftqyuz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cbqkwlqh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bsqnbqor.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rogvunzc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrcanju.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rffgalhg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2botvxodx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2owbibgyb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hhquifao.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nznbysom.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pfohvbxv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gqgaknwz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lsphmwsr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xuttbmzn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqpsudq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qpndyvax.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2sfsmqsko.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2axpwzkhh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uasprgis.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ndkudezf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2tpbpuzyu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fivwdxyz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2becfffsq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gfylhlep.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ydusaskd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbmgxkgl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yutfvskb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wvqtahcg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2odopeawx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmadjdvp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wgiarmsk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bkerbfwa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jqyelkio.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pmmgdvcs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kasfkrva.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kdsqmikk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bzepwwgr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xloszksf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vhvoovfe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yeiicphg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2oejukcco.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dfsguecb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mwmozvzd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2mmqotkkq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2oedgippb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jrlabqdc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2hcdkthiu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2seiunhuu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qnkwgoaf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kbauruph.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bkfxrgqq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlqlcfwc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mfstiybx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kkpvcyxo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wowjmfap.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jslqkadk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2goyfimxh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2aowzxpne.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nyjzrxon.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nnfmrjoz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ocxyuzzo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2oixxjzud.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvpzumy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sbwnhcjw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hwlevzad.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2znhqxajn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2niforxov.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dlqpnpbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mdvsclnx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jmergaus.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zmgauckj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2aistrgoh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evbjbmyx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pgxwkldm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ojdzfxqt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ofevncur.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kfeluhee.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fzciqntm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nwqzilwa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2uxrlqacn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2cmdqbvwm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qiiniofh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sidrjcpm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ntudtigy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vtknpqgx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjdbyyk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvkxfbh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mcdukrle.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mjruilzq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2shtezuht.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rgkewcuc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cqzkuvom.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kyxxliwo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qocbkfvj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rjyopigz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2syavbzgk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2weqqjbfw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cbxigdvj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mtxjyaty.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2drzkoqkv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlohlceq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zaynnhca.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ciakioef.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yydtscah.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uuehhzbh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2thznqtza.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zottnxmk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qlorlynw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujktqjoq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qvbjwhjs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qlrsrhwo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2leitvtva.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2szhphacm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rgxvrnci.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zoumwhnq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pzhbqexx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2opeakaan.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhaqardf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dlqyvfwd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kzcledio.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2fqtzhcdj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2sclhlzvo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2otrrobqv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2oxquqeew.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cnaimjgb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sflzeywu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rwrumgkb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2epgkweoe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2aofueehh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ebkfzacn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zalxslqj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qaouzvfp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fsbwtxdk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qlrhjprh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2owhlmcda.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hzknjydu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2esgtuobk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dashdovq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mkmmpiqw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dzkvaquk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2aabaenbl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqmhwfam.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xpmmcikg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2esuvxvrj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xowwwpty.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2fpkarwlg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dlbwgizr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xzjztwpp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2igsxgnln.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2sssnjeco.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2htalyyzk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jlopeele.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdnfkkex.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bfoctgwl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2obygpywr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xedduaca.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2brnvuwdn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rgvnykjp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jeaopkjl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mzuiigfi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qlnkufin.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kuvvoiwv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bxpbyjaj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qegytezp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vaimnvrt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2izmvoqsl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdxhnjt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhwvjamt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pgazpcpq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hynjjlbm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgdnmaut.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pktjaqzg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmdvqrz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ssaeecmi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qwuirjql.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2exmhgfvi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zemcpaal.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hxmkyoch.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jsitwzdv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2otujilig.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zrzydfdy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lbukoyee.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cxvlyxxu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vahyviad.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cilittlu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ynooyvrb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ycmdmoqx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dyznmtew.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tnvlgqtj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ryslvrxl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cawlkggm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mjarzqxp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xvqupsys.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ndytsdcw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2iqvttcqp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ujgegcxr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pzeuccgf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2gesvkwlw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bebguqjs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odhuhhmk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ggdikviy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bggljsfn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mucwfrmo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wxyumpkh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vjkaxoxp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwrrtjzb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ioewfiti.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2elykgxno.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2flvbbrpi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zedruedy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qhzlxuhg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fnrhkgzr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lgoyezku.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lkfbsqcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2paslxulx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2llnwcote.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdthrytm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ghtderif.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ghncuopt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2adewrigg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uakdlchx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2labanadx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nbrekcrn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxhpnmqc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cnefiffa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bnfrtdil.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ddintwpo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nwpemeys.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iwmnrpun.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnoloqqt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2blhnlrgs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2elutkhgw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2notwoqoq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2olrxovev.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rxnjzwbr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zycjxndm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ftgcihpj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sxazqrva.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2afybylob.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dogmbhfo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ccyckftq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fpixejuw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zgwqvxvq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uauthcig.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vuqyjyee.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iagyvtta.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vhttqcyl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfjfxuh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bjuzzwnp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nnhkkhab.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2vmgckvvt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rzurgegt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jnuymkxc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dgxekjyy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2heaqarsv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rrdhrlcf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ostpslwj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ldritlot.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yimevtfl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ozkfelhm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2svxrpzdu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vkfatdaj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zobekbvi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njtbqrwb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ainqlyxt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iirdodyj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dllqpfoi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gioycboe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nixqymhq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yddyiunw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2entfvmud.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xrlulmbi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2orygwkcj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2adewpsok.html


<!-- 参考信息 -->