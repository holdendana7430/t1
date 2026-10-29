代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gyzgheifv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/grztfibsr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gawjljowg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gqwdybevy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gfgkejbcw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/ghgmgksyz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gsetqvcjd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/glqwmrlxw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gygcpggvr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gawcgzedz.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gzbxlempr.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/ghqkjhmvk.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/goweymobp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gtlzvjknu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/geqwbhjmm.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gvvujtbck.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gdjvqtetb.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/ggupywgqz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gprjmlsbi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/guuigwsle.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gozizryjs.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbuzhwlmm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ggovfhsgo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gvusstssj.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gsijyuezq.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/ginaobszk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gmjdchbxm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gnsfupohg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gjxiccchs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/ghfanbqku.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmgssxdpc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/ggpycodwo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gcblnmyhf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gnzxhjrkx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/godosfnil.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gckrlykjr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/glebkxpit.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghsvnsaim.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gnfijfpwd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gvpebilpc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gpmyvzxnt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/glvlakzre.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gyiozzpff.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/genfbdxex.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggihaojil.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmrkinfbh.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gfpcukzmj.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gefrmrkhv.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/georasklj.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/glotmsclu.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gaqjhosum.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gmtxbirfc.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gfjsntknn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gyjiesjzd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/goaarualw.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gswfxmqqz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gozljqkod.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gpstmgtug.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gzawtxvzy.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gjteymscr.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gupdzohos.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gdqynnilf.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/grkkzecjo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gxfuadaha.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gneqndlyr.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gucirlugm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcfzcyhsy.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gbvvqamyj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/ggdtucyqf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqamdouhg.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gsggoojel.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmzimnfrk.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gttxcuyiv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gapenrcdi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/grdrksdva.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gwjyvjmng.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmcsqpagd.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gpakukmnd.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gelqlqadt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gfzknxecw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/ggvsfiyah.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gpsmjomxk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gtixorxkc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkectjntf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gnjqijbkk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gxdtatytu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gxjxnwpke.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gjaqinvdk.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gjwbxilxf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gwujigbzi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/glcapppxv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gohvmgqss.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gbhahnwke.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gpqdljxhf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpoiprkts.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gyolvfsrx.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gmdauzriw.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/grkjmvyzx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gftveikao.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gxiauqvyl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gfegspwgi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbvtpowbw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gjdjdzuiv.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqsbkwgpo.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gwflfzkys.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/grbbyobjh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/garjabpve.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvhtspfcu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gwjusulxk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzdkhtoxe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gnvhourih.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gihesgmzr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gzdfrzsfb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gfkwsgvev.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gmlhrfuyz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gfudroqiz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gdxeicguh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gfrglhzws.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/govswigod.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/ghurqhpdf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gajljvupe.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gppihxmly.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/guvhwwvbx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzkpwnhit.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gitkdkijy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gjgdqwgvg.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqekzkfnw.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gapegjpro.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gxbxxhufa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gqxculgqd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gwbmcmkhk.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gvfvjfqft.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gjgxigkbz.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gkbwkimaf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsgyqovnf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gctyooakc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gnoudyvvi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gaigigfzw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gzxsvgtgb.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gzexdykwn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gyqroptde.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gfyqbuijs.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gjvjuhtdv.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gqeroajma.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gonqmugst.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmlwdorjl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrvddtmf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gbdxzzybz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gqnszwdgw.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gybtbkyfj.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gglxiusma.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/grphrlziz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gvfzvwzjw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gyoevxekl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gcdsaaric.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gwnwncehg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gtlrzknrk.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gwaxzygwa.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gxnvdutpl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/giupthmmk.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgokipv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfdplbeba.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gyqsbezel.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gtxcmxpip.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gmamhppbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/glartpugj.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gmrrxbhcm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gbzkscjkg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gnoyhkvyg.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gdqlrjimd.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gjgcyzzsz.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gfsdwzzwl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gafiutscj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/guawpaxen.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gtznbvnco.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gujdhuuxb.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gcgzucfrp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gycubgzbq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gezqjdlne.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/geidunfsn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gxezaikff.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/grvpuxuop.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gcnemxpoc.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gjvvplisv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaevbzrrf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/guxhaxqha.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfsrdzv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/ghcvighuy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gqozmnxte.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/geybwlrzz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwptvowcv.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gaclymmbq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gcjnnlpvr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gnyawvidm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/grykkxsmq.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/goqzpokar.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gyjjnvsof.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghordkkdb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gtqqhovpz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gicpurjxt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjwgjifqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gfrutxeam.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtekdwqgo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/ggauwuaic.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/ghrzenawi.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gfazekvvr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gkzkjmudi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/glzvnmeqb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gxqbnbahj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/glcspvigj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/ggdlukghr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gjymhcakn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gnoytuwaa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/glulqtual.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gizowwpnu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gcxdxkhmz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gxayjzovq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gjeluepww.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gvlyxlwtf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gkzuhdvgp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gkrrdtwlm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gjnqidusi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/ggrmrgvuo.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxtbylccg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gogpmcufv.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/guwroemby.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ggoynapfk.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gburyskrb.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gjxzxbwqe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/geclswgwy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gunkgplmy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gpdauwkfw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gglyncsbq.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gmccozenf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaxvvicjs.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvdvvuicf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/ghqxmrxjl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gyivxhjxk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gskjjqtqh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gunyaanqv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gqhnzgibq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gzzbvcjdi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gxdlsrwcu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcbiahznl.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gcovolzip.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gcwmjjwdx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gzarlgeah.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtvfwtpf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gftyaapkv.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gnsdfouhd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/godoigtkz.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gjrmirgem.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/glmqauvon.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gjnwzwtqc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gwpvuzgjb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gkpnyjnat.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/goumggfdk.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gymlugbjc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gfearyjuu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gbidszbzw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gldvbxyqy.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gdljhjiuj.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gfenkahqr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gknzlktei.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gzitdsjsa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gmlugngir.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gqmrhmmsj.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gjftucfhh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gqfyivkxt.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfwnumbwv.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gupcwovhq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gvamsmdep.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gefzxcevb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gtrbcpefi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gpfhsvezm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gaectcsce.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvdvblyhl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gmkjrhjdf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gzwdsnlth.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ggrqkqtgt.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gbreybzke.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuxxkuyy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbzdjmtp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmdjeobtu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gofnlgnxu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwswfttuj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gfbnwmulh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gydirwhcr.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gfhslnxnu.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gnyilzkuw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gkeoqcbbu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gtgqqfbji.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/ggsnircmo.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gvgxzrzic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gewqzrvrc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gynpdmgmq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gucdnmxjx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gbshthilp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gosislxyq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gvujiafoi.sHtML


<!-- 参考信息 -->