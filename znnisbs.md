代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gyewpszbe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gdykeefgn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gxnoysufe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtbqshcaw.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gpkoipsbv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbnpfeqnm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gywyumsvm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gbjlxpfez.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gebuyjlrh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gkkxcpipg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ghisjwaic.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/glkdgellr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gxphzozuh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gipisnkph.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gxtvmhuob.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gvxdhyfhm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/ghymvqorw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gtzmowyfp.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gjeaodmnk.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gruzfekjm.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gflatvoye.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gtzmfiago.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gbkuugpta.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/goxrbmuqh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/guepghlsq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqycwijuv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gtghhvdzc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/goofblimv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gmyvmttye.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghfvgpieo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gigrjphwc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/getcgxebd.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/giaososnq.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gvfagfuoi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gjsxapcxu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/goglgequl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/ghfzeqxrk.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gvtesfdlm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gxxchvfdq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/glmrqmokf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gpqbapjjr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/goqquimpq.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gxmeqcqgm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gxndyzteh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gyejlqvzr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gmkyqmqsn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gypiykbwa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/galxcpcft.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gertmcrax.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gveaegcfw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gstieliis.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/glsoaocqe.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gowxnkume.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvyisgttp.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gfnzlriht.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gcacxnafa.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gmcagrlva.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmxdveyca.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gttaraeox.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/glyzfssmu.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gsgznwlyq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/guukmskdv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gystnrtxn.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gxqhqmovs.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmkfzvift.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmpytruzq.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gwqwnrgva.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gqljceltv.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gjjplpxsq.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gfztsuiws.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gtsmufcgk.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gfoowonhx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gktvgpzqw.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gnmkfweuw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gesnbgqyh.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/ghomyupbm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/guqjkcunl.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gxpxdjzoc.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gqbqsqaon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvnveljlx.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjgpsiwut.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/geyqmezis.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gxprebaxs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gymvvrmpb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gyssxjeuu.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gpkvgcfkx.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gtxmodjes.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gqvxxantu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gxskzisik.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ggiagemar.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgttyaav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gzjlqkqaz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gysqwqvlu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gnqmtjing.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gdsiqecpe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gogxoarin.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/guxdkdfag.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gqheyibwm.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/grdsmgvwi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gndalpbso.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gpirbvadk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gzauwavpx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/ghlsefhqt.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gzqtpvbuy.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/grihorwpc.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gaecpqhpj.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gwkblkpos.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gspsayrvf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghmtfiptd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gltabezhs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/giuqohqbu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvjmjvwaj.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gtowetrau.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gvtgoiktp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gjgymqbaz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gcfegijzj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gikhqhkmm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gblmwnshs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gnqzfryem.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjewyrjbp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/glwnkhrhk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gynzkwqqz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gkyfjqnmw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gjyaqdbmo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gmzivoqos.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/giclkiwpj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gedvsdvck.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gwrwljxjb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gulboegpz.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gixivpbhw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gvvbwddii.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpnggztma.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/goplirlqe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gfzmmhznm.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmswhsryk.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gayogdqxw.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gmqnmzacr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gkproyarv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gbypnqqjo.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gkrzdpocm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gvhcdcxaq.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/grtrzjjqd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gxyilscrk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/glksbonmx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/goeefvcrj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gcskhgoxa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gqtwiggnn.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gszkdrxnt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gezrxxpun.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/glkmzchiu.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gfwybppxu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gybhapgii.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gcsmlvubj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gtxvfwoan.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/giyuoubox.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gdwywzaqc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gjhdmkoxl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gzirmwyfr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gnbsmkmxt.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gwhyfwobd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gxzpoqkxh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/ggfvixyvg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gcowmudic.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/ghffwmjsq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gosugqatm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gurolpywf.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gosncxzli.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/grlcftfxg.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gmutioeai.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjgzaqxsi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/ggmhgkpao.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gnprvcace.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gcikjhkjf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/groxzefnp.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gotcgyqzd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gtwcgunwe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gqpusceak.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gmlgvbbfu.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gxaqbttkm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gwcmljual.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gfravkwua.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gxhfwvvul.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gdaggaafr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gxmrxljvt.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/ghaicmxbf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gzncdnxaz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/ggyzeiplr.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gqarsbgpb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gsimngcqo.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/ggwrezale.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gfgrcrlpa.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxzcehpcs.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gleptkcpi.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gtotbbmaz.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gohfgqblj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gpiayvpjs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gjvuqoabd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/goyirewis.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gjdblsdlr.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gridsyyuy.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/grredssua.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gkwlzbjle.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gefhcyepe.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gciluckqz.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gpjdfvfhw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggnyqidmt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/grneejwah.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdygjavak.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfzidxhsc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gfzxamkzx.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzlofcpcy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gtsnviisb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gujscumlh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gbjygjlel.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/grnowvkxr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gwmuabajy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gswpfluzy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpdihqqrw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gmsgwpjgg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gdkplumzf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gxipmtidw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gupixrtif.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gsptxyzrp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gqtcizven.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gvquemvez.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/ggbwhzttr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gkvahsnmt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gjzgsuheh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gqluieyjx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gtarwhrpe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gscbvddcv.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyiptivzl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gyzywtquv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvqrylgf.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/geajrpkjv.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gmvrapdcv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gijvvqwog.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gjmfytder.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbrtbczjp.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gzphodccg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjrtadkhh.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gqpzbvkht.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwnxldpfl.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtnikfbmk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gxlapggjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/grhpqvslb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gwoviqoyd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gntiidrim.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcgbmwg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gircohksd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gvjvjptbn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gugfqkvxb.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gipyumrxw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gvxoupadk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gelggnvsp.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gnecjrtix.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghyjeoodq.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gblhcnjjf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtxkvmett.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gngnijtmw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/ggvpxmkbi.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gljvmlezf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gqaefjyja.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gdamocndx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gljymwfli.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/griazvfoi.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gzemtxqjg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gpmxsrzdr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gtfntzmaa.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gzxwrjrqx.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gskitiars.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gfvlechri.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/giorhogqe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/golyutlpo.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gihdqvcdl.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gpyxnzeio.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gjrcczswm.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gfvrqkips.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcjcdefqz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gokcxygcs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gareiqfqs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gzxsxoxpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gqvvqsagm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbudzykep.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gfcozsbxw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/ggmvmrygh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gubbnlkta.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/goclqqaiz.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gnykenuov.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ganmwylvd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gegifyest.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gkyngislm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gaklzrzfv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmrkcddgl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gxgqrqwns.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpotqysne.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gangaeovz.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gafcgroxy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gtcxjugpe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/guxfqkxdv.sHtML


<!-- 参考信息 -->