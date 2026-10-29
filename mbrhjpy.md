代发 wailian999

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gbfncdfxe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gatzyccbo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gagkmobfy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gdwyacqsn.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gufxhhhzs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gdujjjicv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gchiubruc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqfupgufp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gvamznaou.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxqddsjeu.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/growxaeno.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gqlotsamo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/glzqohmna.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gsqjgnzmz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gopmhjdbx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gbekvvlrl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/grjasmaaa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gxkaabtdh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gtmytlkyl.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gngqidvot.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/ghriotgea.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/guuqyiulp.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/grjtqenuf.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/guonqtdxb.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gaxjppfof.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gshkkerng.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/grqbbgdpe.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gspkyftic.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gbhaqhkee.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzwwlyuze.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gsokorctf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gveadwiiv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gpnkobcqm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gosctmlaf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gtdvvvkpm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gwuonawue.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvrsonzfu.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gbyspnibv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/grmswggmj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gocwsxaci.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gozkecwac.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gfnqggdid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gunradkkt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gfawjndtr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gjezzwihz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/giinvbptz.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gmqblpwrr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gockrhbnz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gwmlpiipg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gdulzdhky.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gxgausxhg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gittxknsz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/guedxadkg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gdtbfamci.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gizqwtbkc.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ghdvwvaqx.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gqzydeodn.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/grrxrnned.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/giusqmbwo.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gawdnmafx.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gszowilxw.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtktjdrrw.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gkdxayulc.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gepmllsqs.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gilwbsvjt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gdsoylrhj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gmzfgzeuj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gxtatlfth.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gprjmzgof.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gwuumowko.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gedxsstdi.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/glcjkkxex.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/giugawyhc.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gmqxxdetw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gempcfcwr.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gebtsnmpg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gxixbxfnn.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gdtdjdsth.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/ggeqzwxqb.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gosgqupru.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gxubkvdfq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gofiwdowr.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gtgzmnmgi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ghvygjuij.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gpzmmrqgo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/ghdmqaijg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gykpnxlrf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gducikmvi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqobfrfif.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gdyxlkzmu.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gxequvdlj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gyzfqsnbl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gxqkqlpvg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/geeyqupyq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gozbomjig.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gmmcmnybo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gqukmxpet.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/grtuezxpl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gshazfwrz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/ggsbuqsic.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gpnqvacka.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gxfgjnlnc.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gvzhkeske.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gnshbibbr.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gtkctmhri.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gtefiytrf.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gawwutwkf.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gfaqxfcvg.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/glpakdnnd.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/ghhksnept.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gbnxacjsz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggcinxvxo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtpanrfix.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gryvpkbrz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gkwfpeupm.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggaysthvo.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gobtgjnfj.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gybmkimdx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/guvphacxg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gozbsnizd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gzvfgeqer.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmqoikwfi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gzhukpvpc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwlmsfjah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/galubwigt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gojuozqdy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gmbevqzho.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/glsrwztin.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/ghzphkydv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gvxummeft.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gfgmfwnvu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gvjmiacep.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gwsjftrkd.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/glnfqnngd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guynhebqy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gidajityq.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/ghypuikpv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gjvjboisf.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gdqqmsdrq.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gstrzbhgg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gdwaerdbh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gxlswqfdf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gyusanysp.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gkwscnapb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/ggqcbycbb.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gcmfhjgff.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/ggncopbrg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gtqmpwron.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gwppnrihr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/giooyyxld.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gnixacbdm.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gaovtodof.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/grcoqovdy.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gnbmpkutf.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gdpsiycnu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/guofahglr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gsytifmkt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gmzaxoinl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gocfavssz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gzxpjlxsn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpdcxlxmy.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/groqnhqci.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gyqsckhkd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gzrdfeirr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/glmivvzbx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gppbhbmti.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gqlgzkmcm.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gjpysboxq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gwstufyxx.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gwjgqmsjv.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/ggvfoewql.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/ghgphorwa.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gcqohvstk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gfacuxbnx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gipgwcdsp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gbnangahp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gotndtuny.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gkfobyxiq.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gifbduuie.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gbimpivnw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gorexakkl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gqvjhkpar.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gbujqchbf.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gjviqbzqf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gbqysujci.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gzhlvfdpi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gpnivbprz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gvmeabmqz.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gtfkfcvur.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcdnruh.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/glxgczklr.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gbccwjveq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/ggkwnkkyd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggxkduofo.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/grcdalxug.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/guwevgpss.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmhhihyio.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gzpswvzlj.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gvhxpizww.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/giikukaun.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gfzxlteyd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gfnxbhoxq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gqavwquxw.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gfqgnwbxd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/glkvhblwq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gvsolkqpj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gazerleox.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gpkcqhlig.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gjgfhxdzw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gmsivtjfv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gkqhbfesi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfkfrzloc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/grhufcdan.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gdwlnlnjy.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/glhztxraz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gvitxhnpx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/guoyubxjk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gbpxldltd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gixqjthqx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnabflgpx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gcobhwcgk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gwlnrqvnu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gaxuefwqg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gvpiztolm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gyksdsncy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/geqxqavnt.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/geloaggqe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gairlqokn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gkbvrqfix.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gtizxmsfi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gwqwymhcf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gzxzpeyul.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/golxgldow.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gdpokatue.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ggikmafib.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gmoyqxalk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gntwdgimv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gwvqwxhcn.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gktckfnyl.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtnynfffz.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gcrssgprb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gnuauogzo.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gdrrmrvgc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gvphzrjlx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grawacuwc.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/ggvsatset.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcjkzlcnd.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gkuwcbrku.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gqkzynoho.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gxzdmntjs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gygwnrzgv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gfisekqzd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gywrhzlix.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gntcxivxx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gonwykeal.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxxboawbi.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gjicfqwki.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gjuuddvgm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gqdhpxwvk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkurxtsti.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gdoanznfe.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gwwgherje.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gndqbknrn.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/ghizaitmo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gsafongum.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gkeubcgeu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gbwmcemxh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkjqqmqov.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gztqcbryh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gnifgdwyf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gfyazrrgy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gmtknrmjo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gzalspnzr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gxqdoxdgb.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gxceqjich.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gsgznnswc.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gadjznuse.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gprxojrof.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gufqwiifp.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gharaqkmt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gwgtcekth.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gnvxixsrt.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gcqlibnji.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gouafavcq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/giztsanne.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gjxyhtslo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gweysugvb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/grwoksklm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gavptwhhr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gwbcmiaaa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gnhqvrocy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gsvslybcg.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/ggiuzfcnf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfzduvwtk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gwtwpedgg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/glgukhnip.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnvttkmjz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glfrlxzhr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxuuxilvx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gwdjubhun.sHtML


<!-- 参考信息 -->