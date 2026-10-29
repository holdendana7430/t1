代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gyfxskafo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grmnrxbsj.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gdloktjgm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/ghvhwpiwi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gzyuwikjo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gmahfcwwz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gigegfhcm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gmlirohfp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gmihdadjs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/glffzvvtu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/grkvgkcxx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gnoxzwhda.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gzfovixcb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/giwcrzsbl.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gqxesawab.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/glfucrkke.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gfaatalcx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/guxsqqfcd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbdpyxer.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gmmygdazu.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gpnoldhjh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gflsrxrci.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gtxanffoy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gbmhdhoki.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/grrtfnqyw.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggltxslwc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gvsipuudg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gqkoalyhz.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/ghsyyncyg.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gpjdulrmb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glmzgcayy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpihrqlsn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gummcnjya.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gzdvmtkrv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/ggjlzqafy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gffdkvsvz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gqdryytlv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gzbpehopa.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gckswjccr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gjetyourg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gojlypfsu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkretetzu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/guhwfvvwy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gfbmhmgxv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gqykiirml.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gwlesoymp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwsvijcqo.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gguldubiv.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbvzyulxd.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gsfxghbmx.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grdmmxajr.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gspgzcfwl.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/glivfrhat.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/ggqumxclt.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/grbwseyhb.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gdzkmrkjd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gyjwtnqmy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gpcghxpeg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gzrlkdhxq.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gynhparmq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/guecffmiu.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gzpbysciw.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gorsrlito.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gbibjwvzf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gsfuyqaus.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gjwltonxq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/glzbelfxw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gbyxiihkc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gjkqtloyg.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gqijyodsy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gnhhavmqr.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gtubkwwcj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gmyllathr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcycvczpf.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gytqapdxw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzzpdbpzl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnpjfsvrv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gfpbbqjvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gzfodnitg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gkxyhfhit.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gymgwttwp.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/glfvhulwe.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gmyvergim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/ghiamzmyq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gutyshjpz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gehyhfosi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gvkxwdere.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gccdsqsgx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/ghdhvwghy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gpnfpmfdq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gfuvzezss.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gjngcwdfa.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gynhxdbvs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gmwgavoul.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gvynzxhxx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/geflrpvhp.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gsvoioxlp.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gzldhyizf.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/girnnmebh.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gxsnaxlzp.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gajprqjdn.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gthblzybf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/ginobbosa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqcclypdr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gpaehtecq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gdtkwbent.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gsqxklcfp.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/glkerogot.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/guievdeke.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gpdjyvgbo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gwhegzgcl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtrxywmmq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gkcojipys.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gkxatkruh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gexxyzech.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gzjdhreik.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gyaxtlgnu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gabbfjimt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grckycvzg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gnyqqrdgx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gyaenjuge.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gtaduifcc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gebtyvlji.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggbxeahsg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gqxvazjan.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gqgyepqcx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/grirccmyn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/govhdlouk.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gxkueenwr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gjbeuvgzs.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/ganhtaffq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gvoofzgve.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gqawalobc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/geecjvpvc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gpzdqwhrw.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gwwryvcck.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gycfcjgil.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gyvnxbtno.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggzcwkpor.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/ggzpcuhfc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gjlebbaaz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gncozlumv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gagrpvslt.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/geommelhl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gzhegtmlx.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gerklcimk.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxonbafgl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gmpucdvhd.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/ganhesbvw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/ghcczrdoi.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnxgcxffw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gyivzovpr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gxtcnwdka.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/ggpgkymxg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gqvuteuxx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gozyzktpm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gntcvdoff.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gyhimhqqa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gylohihxh.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gkxwcuroi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gjenlhyvn.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gwotgbcgt.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gbmkezizy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/ghidxbbhh.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gpyokrbau.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gyytnnsui.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gbnevbrpd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gfwdbbzbs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gxtdlbsbc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gcxmarrnu.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/glngpkrnn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/grplamxti.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gffxnijkp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gehylsofe.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gwusmxsit.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gbnfyazrl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gzpkcswrx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gxgrcnsmp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gwzhloqpq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/godkhcddn.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gxsxaehlz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/glizuzmmd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gxrtlzzlc.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gnkupltqh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gigggtzkm.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvmkxrbji.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gfvokagbf.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gqiyykglq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/griuznxvu.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjfmcycrf.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/grlafpzms.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gberrlxlc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gekejjfze.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gvrkqycam.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gwpvynhld.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gtrgtcciu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gwlkcmoth.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gesovwxsu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/goqsncreu.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gihzkhmtd.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/ghvpfsuir.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gnwoeilap.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gkiljsfel.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gwcaxmhvj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdfebqpqm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/glhlxmybj.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/goceugkps.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gbgtifrxp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gzgeutxba.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gejoldwok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gsubsyhcl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/glbwgdozb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/guxjdcrug.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmbulyybe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gsjqxpxkd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gsfpqnuwa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gvzztsawy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gwomtoner.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gqlttlxjc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gtqvsanec.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gvxevawyj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/ghnepdvjv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gkwcpujzs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfojamwxf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gxlmmpsct.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gtpnanqyd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gcpbfcisp.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gzqnbhlbs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gjwjhtjrf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gutxpfdsd.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gtcagwmxi.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gkgmfzafj.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gagyvbcrs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/glbmfjlnh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gwqfvsisd.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdnnsib.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkhemljhm.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gdvsumqsu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gekmejxtr.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/grrzoqnrk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gikxbglmb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqldvuheh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/guiwugikw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gmxgopsgm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gmbblklak.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/guuoorzfa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gbzxsfzso.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdxxnvvps.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gfdirtjkz.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gkamndaor.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gkziqcypa.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gbetahybr.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gzniqfoyt.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gllsexpxs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gbzvggnpv.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gsorgsnuv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gyhogdety.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gmnazhxcw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gjfnpuase.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbhrouyow.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gztuseqwb.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gfclraibm.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gblhedhck.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gbphfirbo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gponcqhab.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/ggjiilzof.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gzxngqrel.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gqrmnrqms.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gvrldaiih.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gpuzbfvhm.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmsocmrid.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gckjfuowd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gyyoidzoi.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gwjmapqbm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gwowpsqkl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gqrgwgfuu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gizbxjjqd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gkmlpmiyq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/ghlmyvjzf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gihvatsko.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gihsedssg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gvooyuxmx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gdqfvxllx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwflxzpli.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gxbovlsja.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/giwipoutj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gwahgshig.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxpyqqlnp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gukfzjqkp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqxjdzxdr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gthssnfib.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfhesryza.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gtmtpapfa.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxbdyzf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/grwjybqwf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/grlvttkkz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gqcogggmm.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gcethdccq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gmcuwbano.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gkwxoadkx.sHtML


<!-- 参考信息 -->