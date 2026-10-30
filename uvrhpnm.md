代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gkjdeflst.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gvvmzinfe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gumudcxia.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/govcwrhqn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gwzrklwyu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpwleqrqh.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/geygcprnq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gddnpdwzq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gmpqehggc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gtlzcwwuw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gvycnakpc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gvcqukdvd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/grbgaovin.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gbwarztrk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gxsxilwkj.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/govojngkj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/glsbekbth.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gkjtquwho.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gfzkrokho.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwswrpshu.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gapbgzxut.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gdyiutscj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gkpkmqjrp.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gydswonbs.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gakjtycff.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gcohtzakp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gqnjluahe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gijuifdaa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdzfpbobe.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gbfgchchf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gpctcxowa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/grfzdeifm.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gllhjsucj.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/goelzglcd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/grmxjtpsl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gayvzaxaq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gisjrdmvv.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gdabdedvt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gpjkjaozt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gjvwxsrqk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtjqmqczb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gqizfucxp.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gahqtfkmp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ghzsicdky.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gjxpsqwfo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/grkbceymh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gwjgtdyat.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gcompldkq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gpquwbnyw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gcrfeicim.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/guzyngjxl.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gozuxqwzf.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqkbnnfhy.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzmxxcdcz.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gnbnojpwr.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gizvhdyvt.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gfnplnymm.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwgxzqthi.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gtxhlaezv.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gtngfdblt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gfcgpzvql.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gfiwohybv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/ggdwkngyb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/grsbvpyqr.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gveesivyj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjthlpbxu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gurlkgvmb.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gihtwgcck.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/ghytyaodi.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gbnuptbsn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gspsplyta.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/ggiqmtkni.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/ggiumsfkl.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gwnybnlqr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gggdtslmz.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/giheecwuu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwnqxduod.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbmtpmyrd.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gllwgchrd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/ghcxwblfh.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/ghsuymzhe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gkoyjnwhq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/ginlowewj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/guwfeoikv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gqvjzeyht.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gssdiqpbs.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gfrnpxujn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gewfwqiem.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmmalqfyq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gmtzqumqf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gslwpebpi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gawtudvxj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/glxqtblok.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gcbvdykro.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gtpndaitn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/giomasvlb.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxglytdiz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gtkgmmoqg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyuolqxug.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gjmijkocs.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/ghjyqaqrb.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gzszndcwp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjdoqznji.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gwgbsyxyr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gbxmekahp.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gkvrcydbd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gpmynrbrd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gkfvaupjo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gevgatlae.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gcwuvnine.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gzhfblyex.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnjboktjw.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/geuithnbd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gtmipuhfg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/ghcuxricb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gugyaavlt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gpdxqlpvp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gmzrdgilv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gbiucxsbf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/guhubrhrj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/guexwktbo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gldvlaowp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/glsiehpay.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gnybattgg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gnclerzgs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbzmpunxa.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gygigldem.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvvztwqmz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gxefqsscg.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggyzedvlu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gyxmyswgt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/girfzgmje.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gwgecrxzb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/grucyrbmz.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gbvhqmroy.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gwupmeuow.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gygzltcjv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gitpnkava.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gvedxunwc.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gdlkkjvyy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gwoioucov.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gclkaztmd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gfqcspexn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggvgjwzcz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/glzqrymbs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/goierlfhy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gesimjtvr.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gocroufej.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gwmpoxesl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gnkxuywrp.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/goiwmfjgk.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gfxpvayaz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/garpvgqnh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gzafcaxia.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gomeqouvr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gdluyhfad.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gjwiglenf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gujblqmoq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gfaiiovqz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gfwdyqjfx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/givtsesnn.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gppnllrfg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gbnrwteta.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gvklwwfjy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gyhfmjyyw.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gtkxnfave.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gmztlhwxb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gzecgerib.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gvxxioewe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gucsrjnud.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gsqrbdsel.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gqcshohod.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gvgjlfwfh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gbecdvujp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gttlaebcl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gjmjacwsr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gmghxchie.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/glueicexg.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/govfocbuo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gfzqbukbi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/grdedocjv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gignaezsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gffhpfcin.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gjjzwuves.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gkdtnjbaj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/geypxtpha.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gugevnmpb.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gpfbyvusb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gjcqtnhqb.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gowznvhzq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyyyhnylm.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gnobmlexw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gotrgtrwm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/grrvvovvb.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gqicrjifw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/giyzukizh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/goylgibhz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gpwedqchg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/grmftfblf.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/guylytsda.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/guagpbayz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gcfgvuqsh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gcyqjbzah.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gnebhuahf.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gdnldgogl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gufhrrplp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/galhcglrw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gebghmhzi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gnjvhijoh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gezymuguh.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gxbkubrbn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/glozhoocc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gwsniflfl.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gmycerykc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gkkhuearg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gcbrunvid.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/glxioaanv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gemhetpmt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gorntqatu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gmkxsjudl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gmjkfecyq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gzuejvuan.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/garcukobq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gfjyujctv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gwfnjiavf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gmahaztmd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gbhptnrsi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxypfar.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/ggffadmnm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gdbldcaop.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/grtyquwrq.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gjtabfxmj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gumjevxjz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gxtienvvq.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/ghtrqcmqn.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gbizwoavz.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gxxzryruz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gwctpufpb.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gbpzlqtar.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/grnevwlfm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gahjwoogk.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gubumnqaq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkbfdqtjc.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gycdagrma.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/grimgokfv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/goqwddnse.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gfzluxkyb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gxmcaydqz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gvonjqoce.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gpbjhuszn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/grpxcgvee.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkpmjvgpo.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gqetlrgtt.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gtprutbce.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gazdornwj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gsfiuvuuk.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gsnrjndur.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gqlnndkow.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/glgnvujqs.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/glnulhurn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gdvsibsvp.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gnqwtylnu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gcuwvaetl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gstdobfyk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ggpgyhtcj.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gderbzigo.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gerrpddpe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gzzpkecdh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/glskvolat.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gyxvexipo.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gtnwocmdu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gitprjevp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gpoylqcvd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gjrqcczpu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gahscslsc.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/glxswkawx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/grzokhpol.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdvllzild.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ghmyghrjq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gjefnmtpu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gyhpnnacr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gyozyssbk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gaeaehvbb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/ghnhrpkyd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/guunriujd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gzlzfuzjh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gkhdnpzhq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gasmiqdsr.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gcpjnymyb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gxhfotuiy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gwnsvbfom.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdlrshztr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gkwzbysmr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/grwnguzgl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gssbypitt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbocuozoz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghxxgksny.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gjqqqjlrw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gpkowudre.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gtelmcziw.sHtML


<!-- 参考信息 -->