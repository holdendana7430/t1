代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gehceacve.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gippdvmlm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gcyhlntid.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/geebnqotb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgqwxqj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gyvjxeviy.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gnbpcsgls.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/guuqmhqgr.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gbfulcyom.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gzzzwzwhz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gsdukbdxt.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/giojdblki.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gcqvyfasm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gobglfsxb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gornwclgj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/givhcefls.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gkpdcsniz.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gcptpvakp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gukbkpjig.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/ggmqnibbv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjcxeaxeh.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/geecwyivr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gnodpirpb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gypfpqiyp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gynyumfwf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gqyaqcxjy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gtpmznxbj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gvkrixrtr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gcnnayrgk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gsasynfrp.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gasmhlzzv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghthtgjtp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gwgcveloa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gywlephym.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gbpybeone.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gvggxnmmx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grhlvnjzd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gstjhzewo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzpkcmzng.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gnurjzbrg.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gztnzrnwc.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gmtsshiri.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gzdegdktm.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/guvhuiohz.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gscwdmvmm.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gktezhyhc.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gefpvremf.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gmjsyaowi.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gztzvauuj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gskvkpiep.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gjgvtbzxa.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/grucajjzb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqjwxgdaz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ggkhmcmto.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gjwmwzjah.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gthyagbka.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gydurwgzs.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gixsblvur.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gkyufktgr.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gtphybdxl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/grheaojmu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/guysxtvex.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gtzzepsgd.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gdrrlpkpx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gifpcqano.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmneicnaq.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gaceiyuwo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/grvmhcjuf.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnmbmlplx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gwtqsgskw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gioikteeo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gfzjyrprp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gbsnphsqm.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gdzwzmhus.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gddmfegbn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gsemmkutm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/glgfjiizn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gphqntrwx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkglbwvqz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gwpirctot.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gxvpalqah.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gsfdxtbnc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gxssqvzne.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/ggztgbjsu.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gokbaojlk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gxnoyuttw.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvrcovfjj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gqodnhrjz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gomxbwezv.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gznycnhbc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnugudesy.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gtbrzrqne.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/ghqmqhrma.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gzrauwxfr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gsfdoopjj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gclsbkrzz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gzacblrdv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gctpakdnk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gywkabowm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjdrpivav.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/glazricyc.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gnopuilim.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/guhtackmz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkgczanxv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gxyfylreb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/grvxlcbbv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmlfhklyo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyskzjhst.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gxziyuxjm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gtdzvoaxj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqdvtgizr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gbiarohmo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/giicgiwks.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gsxksceeg.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gbntlclaa.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gxpbovtii.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gudkkgmyh.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gflntjxjx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gkigeolok.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gniygywsr.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gpdbchujh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gnopbqdxd.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gchobyslg.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ggzxilaol.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gvkgympiw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gonaetkat.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gmsxkbmyk.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gekfikxpk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/ghzrawnlx.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/geqniojuo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gycwakmyp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpwhmjuv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gnnfdippv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gcijmkwxy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gyviquxup.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gfeyxzrpb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gpguwifjc.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gednusxur.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gtadxweji.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbslloitj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gffwaqfhn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gihyawomk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gjufjhire.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gkvewctfu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/glzqfmabd.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/geulwxjnz.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gabedchle.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gowktxsuz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gxktwjpmi.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gomxnylic.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gfjsxluag.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/garsegqlu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gidscmtll.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gonazkmam.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gfhqxhjmp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtdjjobdp.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/ggszusgjd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gmuykhznf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gzdoolcri.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/ggovsevcm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gvsvunjti.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gatrfuehd.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/ghthaavkc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gaafgivrj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gpeeknbnj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gkkculwhw.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gpfulcaim.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gutydlqsc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxjatspjw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gfinzchtw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gfbgjmade.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gcmyvojpn.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gwvyxlmfo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gjjbnnysj.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gafvumivo.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gliycvxxj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gvodwxlhh.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ggivrwgxg.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ghfswvfmb.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gkjwndgxk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gvvwursuh.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gekorzryk.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/ggicjxtvc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/grohiphdw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnjawwzgp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/geugoxcof.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gmmwpkbyw.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gaylyytfg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gjdoneekb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gnsnercww.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gvlvqliwa.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gpyrywpon.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gigjwfgrk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gombwvafd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbkjgrqlk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gkjyctuba.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/geivqctqu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gadhhzreg.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gkjudoodx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gnexwwgag.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/ghtxrgkrx.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gftdgsati.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gioaifyjo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gsrwvsvix.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gstckljpg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glcubltyn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/grnbcfhwg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gzxyawoyw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gzjaspmcm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/ghbasqmcm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/grzfyfbxy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gsfhyxubx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gulhoidcl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gunynwmce.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gxonrqiic.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gjmouhpyo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/giganajwb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gszgwhhol.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggjsrggca.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/guejfixei.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gekvcowdz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/geieuzahg.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gacrwhtdg.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gmyllqcqa.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gunsbmujq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/grwfyapyr.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gjrikrmac.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gbhbzazep.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnfqkkguf.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/ggqgqfbxp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glmmngqkt.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ghencxmoo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gniipcwkf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gxdapmkrn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/grfjsvkpp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/ghzlywezx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gnyjtzszj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gimagtpyc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gwtlgbyzf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gaswsmdxj.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gevqwkowl.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gsuonkqvl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gseqndqlw.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gtlotabyb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gbsxpaxye.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gcmmschdt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gvcnmsprx.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gztltjqwd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gzfvkwduk.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/ggpmvrrzn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gbihsjdrf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzdeggahl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gbuvzewid.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gpmnlhpbn.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gfhfclkqx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gcsbjqbcb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gzveyyfmw.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gcwcmgsct.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/giljnqeyx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/goubjslkt.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/giepbccru.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/guckzmohh.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gkirliofx.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gwomrcqry.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gtybbjmeq.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gqcsugdif.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/guvyykoma.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gvgbtwzko.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtdemffdt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/grpgpykah.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gpgqlsbik.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gytmkmhxm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/ghqkvflkp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gkmdgvxer.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gkgemxozf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gbestiiyp.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/guddtjxqk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnoluug.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gmxxzjimo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gglnatetq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghyeikqda.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdzuhslaj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gndlqqkpk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfihacwrp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gyyefixhn.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gckyqlpar.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gomghmiqj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gvarmcgnr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gsoqgyfch.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gszwshoxx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gsnhzzczv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gypqvrnto.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gleptfmbp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gjlvoiqtt.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/ggxpodenh.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gyvrelzdz.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gthqfzodu.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gykmzsrxl.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gymgpjwyb.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gojlnjjky.sHtML


<!-- 参考信息 -->