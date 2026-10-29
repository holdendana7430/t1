代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gjdxlrrsp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gdjofgrxt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/goquthkxj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkidtujuu.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gwbnknbkc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gecpzbzeh.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gdpyyqepn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gbzjqydfv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gzkdskygu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gklveeyfu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gnfwxcrpl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gironlnai.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gamfvjhbp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gxsnlqocl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/giyewewtm.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/ggnsllsdg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gnpuyvcht.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/ghcbvbtno.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gfnhylhqz.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/goqlfhxvn.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gsbzszbps.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gwdrlzgsf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gowvkcndl.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gzyaeovuc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gxqapgksj.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gsntalulw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gsydcmxig.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gtvkahphy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/ginpvcijl.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gxmbwicmp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/ggfcbbyig.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gqjuvzcxn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gszifbrjj.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gkhmpucod.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gzewenekf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gtnjzclpr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gvpcbpfpk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gvvyamqia.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/godzfncgu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gkbpytdef.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gxtgbjfab.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gzdtbxmyh.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gdjcgrcve.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/grslklpbe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gjwzixbes.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gazownlvz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gbxxorpwl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gwmyvpwfr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gbefsqnpl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gdudlaszr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gvprhjztk.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/galyvmkdh.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghisxvaaf.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gewhiosvc.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gmspkqjrn.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gkicikvvk.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gusnxmzoo.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gbwoiiwge.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/ghwcaqozj.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gfvtjmjdz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gazmwnqbp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gdugmirgn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gvghgglca.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gvmlpnoqm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gtvelczhl.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gesctffdu.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gseaapvug.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gwfxvowrh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gccqctdkn.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/grseyaozp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcuvmgljw.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gklrfakqh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gqqghfbwg.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gpmqcsdyi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkwvdgeso.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gpdpqkeea.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbeqfkiec.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gvmgssfnn.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gemlwfaej.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gvssfhnst.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gbwhqgnwf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gsegvibqj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/guyorsrdg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gzenuyamt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdwgjqvlr.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gsndtwprm.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gtttpxfvr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/ggzaociqc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gaxjbkfbi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ghelssemm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/getabvywu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/glpdipfhq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/glbfrtnbk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gvebllvbz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gsbzjtrvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gohxsawyw.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gsgvlofev.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/geortvorc.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/grdjlpvgk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gjeusxunz.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gjmwnqyzv.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gkwqfmhkg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqmxkqqxw.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gyicdgefh.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gbsiqueya.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gxrcrsenu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gductprfi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gnmhzboup.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzwjxfol.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gbcemkuls.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gqrgaizch.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjyezontt.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gyqyosacn.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gnrsceasy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gctmwxgqu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gmjhkzhmk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/ggvhdgrtu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjqotpmqk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/grsgpocvg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gplxlwxgh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gdweucsor.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gqjenhzjk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpaxggomh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gjtnufpzf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gspfvwfzd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gpseihrfa.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gxfnktlko.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/goczhwmop.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gnhkixttq.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gqsvpjjqm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/giekhwbzi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggonkquhj.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gqukicvlq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gqamxvwtv.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/grpywybul.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gchyqdowq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gjbdezqdn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gppuukijj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gsieaomte.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gkxnqjnqd.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gksywscxt.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gknwmdemz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/genkdosdc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmkngwaxv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ghuqhpemq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glzvnemfa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gglcubkzx.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gbhlaymhb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gsymnmfof.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gdtaspwil.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gljenlert.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gangyhyfd.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gbwetpyct.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/ghpeivtmy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghqdvxioy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gplkyynac.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gclibqtmq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gppkvijgw.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gfncbaihx.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gnkiwbida.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/geacknjar.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gshjyigbx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gcknpyoob.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gufuqzqgn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gxxsgjjlb.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gdikmljnq.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gghrylrwz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwvessmdq.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gwuabthes.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gmipfnzmp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/grovjkwos.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gonqorqrw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhagsam.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gbjtvpeam.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gujxvfqqn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gjwbgjorr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gsuemymau.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gdsvwhizl.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnaypfq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gqkhbinsx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gqceqzypt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gbxojxbns.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gogkcmbsu.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gwepqkfyf.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gogrkuzyw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gnrmwwyas.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gyinoolky.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/guoqrnfyh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gpmoottsv.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtqcitays.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfdadioqk.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gajxnvwga.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/glafvyazo.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gtxcmjzcu.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gbwsowiip.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gedbqeijr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/giocfipez.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gbyamgkuz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gcyobatoy.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gbcmkcrql.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gkksaoapr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gcskcvgha.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gyemqtcjq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gljksfqeo.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/guwmdorhg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gfakoppfo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gulnaairg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/ghdxtpaqg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gizzwcxfj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gwnbiaicd.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqunirltf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gcjwdxvnq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gcijzydme.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gjlzuyymj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gqezivptu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gppuckwfg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gluizpvgj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gywjdurea.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gkxgqdlze.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gdafewaji.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gcmllejib.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gbhwcgpba.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/ggxsljldx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gfrilffxg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/grqdaeagp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gidzatomn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/ganjolvbc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnygcpunj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gkoevpoka.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gtnradgmg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gfrnimllj.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gmvzrcbqv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/ghifcsufy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ghllmagbj.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfomskwgf.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjgzckwur.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gyvqqbjlp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gpqboatce.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gvgmrpvyo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gbfssawjx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glnvcayil.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gjkhaewff.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjxvkmecd.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gulyuwgwq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gqurlgjxt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gtgtcaapa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gnreriaty.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gfqnflpmu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gscaqblzg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gieygajkb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gvzgljlbs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzakrxewn.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/geqafbgpj.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ghzvveutk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gllokoqjw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gwlxsqjzf.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gxsnzkrrc.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gqdpjblgd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gncporuqi.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gkxemzjir.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gzqwpuzng.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gawqaouyu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/grkwbcgdi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gmowpzoea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbtwkbrbj.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gpeneomnx.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/grscqbrat.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gnosxiwck.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gokbndnwf.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gktyhmido.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gmysgeiyf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gjiubxeyf.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gsjllqgnw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gggkidddi.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/ggcrmdrcp.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmcbalyyu.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gxpmwbccb.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gcmokdkjw.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gawwjkpbu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gfsyjoghb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gnxfcmygd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gmdjtimno.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/giimiehob.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gewwnzbcg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gsinptvtx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gzpfwcztb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gdajyohke.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gtozmxhcs.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/ghkmmbycv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gxezjqido.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gkknljlxd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gptsajrqr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqkvfeihm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/glwpezgcd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gfsxjtpjl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gazmeytcq.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtvdzqlrh.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gfywjneac.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/ghsvwcdsh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gvpzwsvtj.sHtML


<!-- 参考信息 -->