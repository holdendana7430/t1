代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3flkbzvgg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iyyalclz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vkbvooyh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3oqvddiqx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vxbrylme.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cvylgzra.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3eadrezdl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncxuxbgv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vkcqxqax.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3tfonrxyx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3erpksrro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atqglsnh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mgqxzvhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgihuuwi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yrxcxzbb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jkggogim.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3azryhfyl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vqocunlt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tskvrnkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ydjnfszv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zdbygdvi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bdjariob.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gslcahun.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mvxrcknb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rpmbueok.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ikdzdqxt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yhblfavy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kmnwurmi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ejnhtneo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nyedpijr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ngmmxvyv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tmjdhhhd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yuyohtcn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ugflkvpq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3unsrqeix.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ynfsfnnb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dnvfjgve.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qqthwnkm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3usxokjnj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kbmqxbtu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3owbwhyov.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dkgcsnyv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3arcrvxte.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qunurtqo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ajyhodrb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3brylcczj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3stxbtrtw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hxjbllxg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3enrpgtja.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uqtpzrkd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3emfsvmxg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3talgdldv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bjwgbhka.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fvnvqqhu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fhfrprea.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3oimelixs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yfiurvdx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cqqybylw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gjimnodh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bdauvatq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ypfjzqsf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jkllyfpb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dwuzzdme.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fcrdiqwd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hvhlufwt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zjtpdmfz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pwhdrjgt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3acfzhdey.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3neckrjkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uxyzafhq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hcruenzo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xxrfxdid.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yohfmbuz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3klbqnzsz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3bcrxdvil.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bzcvyfif.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fxxfrzhz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ehixrfpa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqeacle.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rywkwcju.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zuzierdt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gglmwglt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yaumnrci.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zygdcwpe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pipnyddy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqdhtwdp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3byuhzpyy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zchqwtnt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amazpakq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jfxkqbdv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bodvsdwk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mbyfvmne.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3niuhtmzz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zvqhqjrr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3exrftcto.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yyyltqwk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mhpgguyl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrxijbhc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ftdehptk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnnepri.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lmuqfkxs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cunsdkur.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3phcwmwvj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hlwqvnlg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3waplyvfv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3onpfwzhd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vneeapmd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ojnaaxem.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pugopdui.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3eexuwilj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zephrpfz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wqqkfkvj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yriqrwhg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qvdhvoog.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nahcuugj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vyhsfvmy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3codzhbjh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ituiitoy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rolalyvx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3splefmlt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcevvzlr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3phtbxcmw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nrtfdnhs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3atfdxrow.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzossrsv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ermgpvkh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wtpuhnik.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wzjcgupe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vqqozflw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3faldiykq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3invdevwg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iskzjxuh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tnqrxngg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3apdamsjq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ocjisenq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zprkwwel.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3agjyydog.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3goehyofr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bzavuhib.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ihbikesy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xicgehkh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wedqxqha.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhgepuvq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kescpmvo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hxdehmpd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ysqtgrmx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wuaznbtr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xyfjkwlp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fvstwayh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qlsyxjlr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlkqgsz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3leyoiotq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pmxpscjv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwraiqb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lxcpalil.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wgctrted.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zdmyeyqb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3coyawhnh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gwxpbhxv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eaypckes.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqjhwepz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qsxrijgy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hvrededm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qocyhiui.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wgusqxqz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xftkklee.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xzgdbbpy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3oxztrjxl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yepjzmxr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pikhatmp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ongdddgn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nhjlgqky.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vlgtnsrq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wzezvamb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fqiflzzj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tkdtnmiy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jytpstsg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lwbmgftj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qynixbun.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nuyiwpyl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qbocojct.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wlgayfzl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mszonyqc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vsacyuse.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3glywfvll.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3cqrcedab.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cugoqszd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ynpfzegi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xdsamazn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hxwacdfu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ktbptlgk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3faxznbny.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3arcqekeq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ohelbgfv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bwtabooa.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bgelnvvn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qgfjfuqg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mypfghim.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aeiwrghh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tglxwrxz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eycmvtna.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzytpagf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3omgpwsnd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zerfiwhc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fuwtlbxk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3grfcmczz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pppkoaav.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3cauhahfj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pmbeijsu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmmfqzx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kzdeqpfc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uvdpxens.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dgwwycdg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3opukqacr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mpqzrnyt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jicmbvjo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kygyivvd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cvkxtera.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eagmyajo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3shthjqko.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jtsbvxyj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mltscxjr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nijkgbdm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3duxeosuw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xldhwmrt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3svtgzkbg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qyyctjvd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cpcftcwr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hmgslntz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hxtojaop.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3sdilxyzh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ompbfoso.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cgduophk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fjpsfguq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rsojjerz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oqzrbclw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dkrqttgp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ipadwnrh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ergkgpce.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jumtcavj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dqagnglg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vpbhlprq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hoqomrox.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fyoxkrml.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3izasvaxc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hqzddmze.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tjzevxcu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3puamdbgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pppzqjqh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vhojbyju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfykejzo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mxzmgosz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3uyxmolri.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdaddzkk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3btuzywej.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fbrgschf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pehuihdm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cprbrrkk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xrutrhqf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zyyqqhpa.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dzimqbrt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dcfrzvan.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kzirdwjp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3voquvnpq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3swsolgpx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmgzwkqq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfyykkh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gthvehxe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3igzxkiym.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gpstvfgm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3njwjepuy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wronfexy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iowgvopa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xuqcpnaw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rvkanias.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hxoodief.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hkmpmfhn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ygeuzyxg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dmthbito.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sipdbmfp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pdilzgte.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jgedjggv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hmxtvujl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mvzfdjvp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3riisyblj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3buenhvmg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rbuiepjg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kerbvusg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ovflvlda.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xpfylnzl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wmerctqa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aaxkqedb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sbhkgpog.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3segqcnpy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3myhjgqlk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qafijicd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jncizbow.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuuujxl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3umffrdod.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bbsnjoed.html


<!-- 参考信息 -->