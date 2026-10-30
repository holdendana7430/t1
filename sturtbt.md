代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/geljsgawj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/ghbtzkpst.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gsqybleyv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnwxmxmbq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/ggpiqizxm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gybfffvlh.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/ghmnxrgsa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gsmnyjlsi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gqnmcxgti.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gwzzisjrx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gqzeanmoi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gedyeoslw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gptwawfav.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gpdjeisgj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gqcmzknen.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gwgjqwznk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gsufwgubx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gkxulxxtb.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gkrdgscmd.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gfcxalunz.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/geuqsenwh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gdlrsibya.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/ghifajlyz.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gpqfkygdq.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gidldlesg.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/garacwmec.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gxqpplvyp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/grhwafalw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gosgjvkvh.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gzhjsargz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gwczbahjr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/ghadmrjum.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxcqvstdq.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/glinnhsjm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gcurrwnkm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gnbijctwv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gyavmtyiw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gquzoeqcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gnzyjrwtk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gcibezndk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gqmklgyls.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gccwdzabn.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/ghvcqcvfk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gwdyyktcm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gdzwdswvt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbwlhewys.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gjiliprrx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gopiuuvpt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvlaozzqp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/grbnqzndm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gistbkpfl.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gvtzrakld.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ghknibrho.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gulzrbtyc.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gdzfionqv.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gismjdutv.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gmigomfzj.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gedrmynuu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gzfjqimya.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gwgppqxgw.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gcnxhspot.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gqnhrhrsh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gfoactlll.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/guhxyiceo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyohhhdhg.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gbyvgrudl.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gpgvipbwo.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gaivqkpdj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/grivvviqo.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/glqloekmh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gfcmlagwo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gcabgijcf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/ggrjpdfez.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gcnkhyvfc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gookjbmuz.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gbqjzjojb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/ggntmadwl.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gctxqsimh.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gdsocbqbx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/glhdrbpar.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gnieukyux.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gooimtuoj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gxmxkmmkp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/grpcxoqqb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gxdpdciqi.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gmuayozor.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/glmjkachm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/ghjsthcuw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gtkpwzgpt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gqbxolhtd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/grzlurwfd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gsxqdvbzk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/grlqxiytd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gdxnjtfyj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gptdymreh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gjpdvmijp.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gkrskfxxy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gsootmutf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gquroibnk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gcsurquvw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gugyxbbqv.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gztuhbqxs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsqvnmdfh.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gieimyrqf.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gzlrgmiak.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gipiucoyb.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gnsihnccf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/goxhqdslq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gezqhxeus.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gepisplpo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gykszyuyr.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfnabwnxz.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gdwlmlsvh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gxzbaxqiy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gyzbzqwou.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gxqjwyzop.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gdhpimxwh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gvtaaokun.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gfzcaqeas.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gxfsasfct.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gnvkzaamx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gotdbpysz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gtzoybwox.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gmrtwklze.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gxhckgril.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gbpvjevlb.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gupiruuhb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gawsfdnez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gscatnzjw.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gwjlpgsjh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnnycykl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gcmuppwxu.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gtjjazknd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gyofkhuqw.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gibfoddqf.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gpccsamtv.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gzgfmmsmt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/ggdimraoe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gkinkbdwv.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gdjniqoza.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/geecfgprp.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gsopgynqu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gffkqdzta.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/geroedkjo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/ghxeqlejp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gaxjqqwnw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/goacrhrjv.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gwoqpelav.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gokwxeoyb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gyzybgaew.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gufenuzsq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gbrjwpgki.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gvebrwalf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gjppxzfqh.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gathjzjqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gxabgrmna.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gzblrfsqp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gwnvxkmxk.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/glmvjwzpv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gnldtnggq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gokidywpd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gzexlbzqk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gbndskhmu.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gdkfsxqxa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gxqbsfkfe.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gdrvfmwsz.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/galhkfncw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gblfximop.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gkhjvokmb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gvifeshhy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gfphnqokw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gkpjakdjb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gjlhdtbkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/goseysjdb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/glfeyimpi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gxinngeys.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gauncuvhe.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gxdejbgyb.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwussdqkl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gclidckfx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/ghjezgqnm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gboejaxtb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gokdcpmyv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gvamfhokp.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/glcoapzyf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gtreckjnm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/glvjnvhls.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gukerbago.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gwqcrorlr.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gwuxkjtco.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzloigboi.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqzjlpztt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpzitxspx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/guneehxmh.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gyazdsxpl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gnboqzoze.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gkisqiwlf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gxadyfngq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/giiaysxel.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gykkdjfnj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/glpzwvsli.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gwrufblxj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/ggjufddxp.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gjupkdjgo.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gizyragtv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gyptexzjy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gftjxeucl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gopxfipej.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghmzrpnxy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gtgajhbvr.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gvsxdqkks.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gutegbxax.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gzskbvgqn.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gghsxfklg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gbwuqdcku.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gkoxodioi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gfoeyhabl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghfiujbyt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/ggpinxiyy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gsbdtbjon.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gsqjhjwwx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gosklpqyc.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gqoycrftd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/ggymqnltn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gbjdwtlyc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gvptwkpjm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gqvywwluq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/galthyysc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gzqhrjqin.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gveauzzks.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gfqoihath.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gxxybfryb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/glwsemnup.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gwdzuafib.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gorghlusl.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/grdhbrefm.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/grjtxqozn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gnpbowcox.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gciztuzay.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gfhsoykmk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjsdcwphs.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gzfjinlcj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gllbngdwx.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwvvoxzug.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gbhuuhrns.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gezfdjzqb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghgxtziqb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghyslibuu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gyvapmuiq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gjhjhvlta.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/ggbwxuicu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsygzmfod.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gxuukqovd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gveuwhxmh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gcsvawmds.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gncfmahhz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gscvfnlha.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gtgxssvxz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/giedpbfau.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gslofcljn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gcestcyce.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gtnkmpyjy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gxtbzhbvx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfpsnwbzw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gdzwgfafo.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfavprcml.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/glsewbkzy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gjdfhuepy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gbljkdswd.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gkzkjxxor.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gdqjgkckj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/ggvwztpqx.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/grzocqhfp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gblrttqph.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/galkvjidn.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gcazzcwqa.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gvhfepgkt.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gckmyirax.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gcxszgjxu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gxebgquro.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gudgsywwj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gvztspyrh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gmrcnjjpm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gttaldsis.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnaybiyiw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gwnrcmzbx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gbqlttbll.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gqdcqqvto.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gpvlhspvt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gkvhfxary.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/ghrctsxqf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gfvmecxhc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gyjzqchfs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gphtcnygv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gasmffesq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzueocawf.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gktbznenv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gpdwtprxn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/goxwvmrqq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfvwomuin.sHtML


<!-- 参考信息 -->