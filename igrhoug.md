代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/grmduhbbl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpuzwhyxr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/guaaryzeg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gueexctqx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gxrmjkrmf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/ghmljqjqy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gdxlvmzzb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gzwfmmrvu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gzjcwbijj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/grrnvekio.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gaqbzdysn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gjixxtjyy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gmyknueuc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxhnbiqbs.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gamwpidyf.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvemhkbco.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gxcxxtpmd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gtezukszt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gspzrhjsv.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwpuzdbym.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gtvqpqiad.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gzbhxpaie.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gtdklipkh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gkwxlbekc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gpxbjdwrb.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gzwdmnxwn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gqwxsduzs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/ghfbbfegy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gegpaqqhr.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gnhudebzc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gekbkgdca.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gfdoqlfup.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gnhvxldnf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/grwacyoao.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gqdnkpqpy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gsbgdofyb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gqeipqbll.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/guzbbklzx.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/grsdppxxo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gqsqoblwj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gthdvlsmd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/geigmcdxf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/grbrvimks.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gtpfbvqqw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ggyjnqmak.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gnduorxev.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gqweejzqg.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gtkcskeel.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gckrorbmj.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gtwmouuny.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gkknzqvta.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gsgocdivm.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gzengtsoa.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gldxetxxz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gqyllebfc.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gstvvpdao.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gooyanpcq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gfgmwptlj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gqpnqniqp.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ggvcxlueo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwdyxckxj.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gowlcvmkv.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gtagvikcu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gnkbmafen.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/glczafzzj.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/grmundvcx.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/ghshmeqha.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdjwuiytg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gyzvligwo.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/ggrqkhkaw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gwuiqiyvx.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gwfocxpyz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gigieyqfm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/glidrzfln.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gudewnccl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gfnctarmr.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gpqwfuvma.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gfkiniscy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhoitxys.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gpjeacile.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gaoeljiuh.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gxsmslbbv.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/ghvmwafax.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gfwpfzidt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gcveodyic.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gbvtqggad.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ghbbvggbf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ggcposzcs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gwplglnld.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gxrzkdwna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gakxqkpcq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gvsdppkjk.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gdqkqlasu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/geikuavfl.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gimkanoii.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gqqoajqyf.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gtxccljfe.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gegqvoblc.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gbmpxslcn.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gcavnulyz.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gwxlclajl.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gegdadpjy.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gwfyweabk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/grfuiqvuo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/grxtkihky.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gmmkcoewl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gzghnwuqp.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvkndlwyk.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gmeuqrlmo.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gblsleqza.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gwotxgvrv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ggwlbnrhi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gdhnytjaq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gpolrwzok.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gsziqytjv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gcsubwiyt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gehvkcpdz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gbuvuzjfq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbmomoxxw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gceetltzs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gslnvnoxo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gbnjdoczh.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gmqjgxows.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggnfutcah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gocukapcr.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gkeusndry.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gwwdssgfp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gyvclqwlb.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gndulrukp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gcpgjxomp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwiplsksz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gvoootzss.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gczncvuhh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gswfhijsh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/ghecpjtsi.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/ggvvketln.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gstjgkvzv.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gbkbqxwlh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gqkdgnpjs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcvxuyhsf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gudmfgkhj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gbkfpeamn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gjvfzbbko.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gcnmsnedw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gvxhppyiu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gugiziuve.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gfngyhjzz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwvhtwxrs.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/glmmfcmgq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grszplzpg.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gfistdoee.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gtpaawvse.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gmfqrfavg.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gpctutuys.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gwvivgfil.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gxnzotxzl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gzrgewwqi.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/goknysohl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gpfsfoykw.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gtwpedtaw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gghisgvos.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gfurrpkgk.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/giabenyme.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gutzskbup.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gvdwcmkmj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gawmfatqt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gffoyhgdk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gbhlbqmtl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gtaaptcfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gqgymipmj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gssnqofpu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gxkhoeuvp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gjdxzozwy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gzqmglwua.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gpmhdwbzn.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/getkhtsjp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gkduqyumr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gfxpfnxlx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gzczkqdvn.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gqqakewic.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gcvwabrxj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/goaghhsgd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gppsumtqd.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gxamgteol.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gusdqxasf.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gsmzjvfrv.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gdnazmwnm.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/giyqeazki.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmejjvlrd.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gybzqggqk.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/giuuxxvwb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gmpipldcg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/grplhszho.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gfrkyexas.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gxffhlrpe.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/grrbcydap.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gokahdsbm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gfnldyyzb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gqztidbkh.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gmfmdlggt.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gwswirhqa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/ghpaivihd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gcrnnmpgk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gilljvboy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gwyipnjky.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/ggaulczal.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gxlsedldf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/guvsvxglc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gulmyhlew.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gdzlfedqg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gwluackls.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gbgdrzdqy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/glneetqwt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gkgtvwlvt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gydteqvrl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/ghfegpiid.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gnixhmrgy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/ggwapexaj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gmeievnmc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gnqmkxcla.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gzdvxdroi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gotedoqiv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gouhfvgce.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gwdcucqoq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gyiyhgwav.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gjawetkgv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gcpnppbgd.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gzxdfhqeg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gicusdczn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/ggbtskppa.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gicgwmwci.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gmdzwqjix.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/ggdkpvcyd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gctyfjiwb.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjuirltao.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gbdwpoppk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfsurktag.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/ggwusqgaz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggndweelo.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gsfbnatkg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/grbbuzhme.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gtyhrrhpc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gaupoqmvc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/guaddosow.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcmkwzoxb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gnxhjheme.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gwamjfcjv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbqjvdndh.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gwkqngwqe.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gdzndazrc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gafbryvds.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gmludgidm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gwbyhuztr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gltqspcge.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gelormwbt.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gqkzjyqau.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gxjyiikjr.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gyaxpzvam.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gdocszrlo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gdwiejigi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gcxhqztpz.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gdyjurbxr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/grcljtayp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gvifzxwmy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gzdvdjbbl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghbdzzqfg.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gylmhdljn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gheupyamt.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gfmbcyjco.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gawfwvilq.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gtxsjafmx.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gmbgdznbz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gbwzaqtky.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gpsjkesio.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gowozthog.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gkpfhyolm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtkyxdujf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/ggbcoqanr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gjizfhyrj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gtpchvter.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gobcibtlt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gokxooqaa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gfzvcfgpd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gregiyvtl.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/genyowitc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gxtvjynoh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gaydmejho.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjkswizlb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gifomkqdy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/geoyriahx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gdmswrhfy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/goctughhu.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjpkyrtne.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/goiaznaua.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gsbsuzbbx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjomovnjf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gnehwhvel.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gzlcxivls.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gphihieud.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gylpzrahm.sHtML


<!-- 参考信息 -->