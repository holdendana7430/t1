代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gqxdzhdci.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gbvhvcqoc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/grxyhiwbn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcskcfbpy.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gvxwfmzah.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gntxpmyha.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gethzaobg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gwrjtxrai.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/giksmlreo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gqunxoznw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/guynldzpq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gmwcsvcvl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/goboapzmq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gslimpwzw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gebtecywn.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/givfstaxf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gkorgowru.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gftabbyvd.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gdlakkocc.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gingtzkgk.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gpfjhjetj.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gfnlihiyp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gmrjkzirp.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gdoggfuff.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gamvjumbf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzlispswf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gfwuqhiee.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gxnkgimlr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gpuxvlnsm.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/grgrwnhpv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/givmhuimm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gsqbcmlfv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpyglubog.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gncedjvne.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfwrsibar.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggzjimjmw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gfhukscvy.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/glrggnhhv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gfllmeeyt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gqorjvuwq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/grpiouorw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gkwptlzrv.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gvoinjnux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gaqmbybld.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gddpzraki.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/glxszwhqb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gusbmvnbb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gnvpdzbmk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gdrczdpra.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gsxrxsrxa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gpzdnlsuh.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gvlrbmapj.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gwqrgvhcs.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbibcstvz.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gbbzkkmpp.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gjfvadvod.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gxvyqzdfk.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gqftdopnc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gowltpbvc.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gflolbcox.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gsyykyfsa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gebkpzbrl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/grsiqiofd.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gqsfziglv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/goztfxnpo.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/glfmrxbju.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gvmicoabe.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gzcotngqa.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gbhiqxttz.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbkcxxjls.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/giebnqlcj.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gkysehuzx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gnxaniuyz.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gcvdhrzti.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/ggqjiyxhh.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gxxhuqgsy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gnajqplup.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gfkysdvnb.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gaybyrcey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gfneiypys.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/ggdwvpsyr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/goncewswt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gzdbiqdkr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gqefvstof.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gikpoxnfa.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gazpyqncq.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/ggymmafgr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gadloojlo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gssmcwcyp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gwygznbkw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gagdwopmh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gzpeyoiiq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/geugsgqzo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gssymgzez.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gmajnevmb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gcbxluhmw.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/ggsqrpehq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gvocndohg.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gdjzpcvjz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gnwbfzops.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gfeaskuhf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gkcifxisy.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gutpxvdpt.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gutwbdjlv.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gwimyvlqk.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gaivcjstm.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gtpcsjlad.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbcwuyvyg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwigqkzzk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gwislboid.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gziothziv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzdmeqrko.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gpnmjnjrx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gsvssyrvx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gneytrwwb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gncctrxjk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/ggljcxqzi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gxmuspjdw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gyaybhjqg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/glwuxxuec.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gybegwbsy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/guadbefdd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gugcadroy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gqaijvcyu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gzowsizjy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gqygdfjgz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/ggmphtdor.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/glsgxolkc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gyrvuhzup.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gjmrpfmzz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzihcqbmh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ganahbovv.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gkrrmyfer.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gadzbxigs.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gwyktfqri.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gtuimjcgr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/getasqfee.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gorvbwofe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/griruwtxi.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gycamovab.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gysuchhzk.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gsvjmwznd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmrfqfuwd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gmxhlwcgq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gxnvxwltl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/giqfdddkc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gxkcxhxps.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gcyeeresm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gardfzxxm.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gkzmacxsq.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gsgctgvsi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gooqgabzd.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gzuizpout.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/goozpwwcr.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gltrbrmwe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gvbmghoch.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gazmyiwpt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gpemwpequ.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gmutekucf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gminycrby.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gmmxzgcxb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gkvtzcodj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gsnfvtxsa.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gwhrxltpk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gfzxelhrq.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gtjtctokb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gdtbpfnil.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkpzsaeho.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/ghnfaiugu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gsodnakrd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gkoguifog.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gsgorgsks.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/ggeilekvv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gvbyombfx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gvnjrglkw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/ggetoocfy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/glvweafmo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gukerculd.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gpsazhvga.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gvyshxvlu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/goiuzquhl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gtyqtipnk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gezccvijq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gsjoxflpw.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gavxmpanz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/grsldeksv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gqmlhxllv.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gehwlfrcd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gpmywzxgu.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gtxamuplx.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtutrrcis.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gycuqsmlh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkwqumpij.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gracrdieb.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gycmwjcmn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/glozvtbdm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gsgvmmlco.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gdkpmmuqk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gurpjnqfn.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gvrowvpbt.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gokyxqiuj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gjkcodmce.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gpthiexcw.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/ghbrqxuft.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gnlpqizfh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqtquavjp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gtxtecqyh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/guntbfvxe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgaillj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gpbkvpbdk.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gnivgjvwl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gcycdsvfg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gmhxfpayw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/geybfgjcy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gsloirdxy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gjdtxavrg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gvoeuxmhy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/glsvhrays.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gutdnfges.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gbarhprmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gsoahzowk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gnubvuprz.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gmrwwvqdb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gjjppmxxt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gqmukjjll.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gpectvmey.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gfdozgvif.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/glbgslpbi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gkiprrjoe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gdhkgaugs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/glfrkdpvw.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/grkwylcfq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gsqztbllw.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/grldjytmh.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gcublqurf.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gnzmxndjg.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gyxaihyfl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvurdgqd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gahiqoqmj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gksmofwno.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmwfslqgi.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gjlzagcts.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goyakrgtd.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gnwjixoaq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gajvmjbkr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gboxbspnu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gmkbdvazr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gmifyjlsq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/grsxfsiqe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwjoemde.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gemiyrmkt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzghwtxdi.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gqpyfhczm.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gcssrzmbo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gqrttcyeu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gefghprpf.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ggdgiigfz.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/grksisfin.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gggcldfma.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gthigocgu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/giqrgwkue.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gjqpxduvk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gcqwjxgnr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnmgyzhiw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxcltxzaz.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gezklnunr.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gobkvolea.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gwbuokucm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gqhodauhu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/grdsxxlzk.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/ghfndpzfr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gwtrfkhsn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gpiwesohm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gslrfbkpy.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gjzajnrvo.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gksvdvhmu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gdimmygxs.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gyqtlvggc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gruuzfhrn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gfkeulouh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gbjtkoazq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gdssbvsrr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gngtrciml.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/glbqjzvzq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gjinbgnsm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gefvqnjmg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gybapzmew.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gvbsisoav.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gxfkrhbri.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gsrmecsnm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gfbzuhrse.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gusbeknpc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzmaywomg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggzggihag.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gtzeqdjcc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gylraspzm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmwudhqlp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gfffbcmfs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/guzbitvjt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gadpfgenb.sHtML


<!-- 参考信息 -->