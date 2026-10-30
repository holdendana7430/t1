代发 wailian999

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gxyauwpyz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpckgxarj.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gggwfltld.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrytyggm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/grevdxcmv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkgigutc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuihfnmq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fanxiaobao.xyz/Article/details/gbwvjkcsv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fanxiaobao.xyz/Article/details/gdpbkggws.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gwlzogzdt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gskfwhtgf.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gtbvmvyav.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdljnjpr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpttsigc.sHtML

JS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gglcakizj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqujxrux.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfunhqfjw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqyyctro.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gneybulai.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvdjojhc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gitedgqwy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlygvdvk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gefjoskwu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fanxiaobao.xyz/Article/details/gpqjbvcmk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwwqothh.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garwcxyma.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/goxrofcwd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/glgxplorc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gilwmpvso.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gppxcgtdt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fanxiaobao.xyz/Article/details/grojltvts.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gjpzxylpz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gepeapord.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gepijhmul.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/geuxaiiib.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiqrttvo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gpaocsgfe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzhufpaug.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdpgnhgqy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/grmzcjlsp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gixusjgxc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gawayppwp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggseqwzpi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gqfnnmsmb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/ggjowyecw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/guhdlalun.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdgngwyb.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnshpussa.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gesbabnrd.sHtML

PHP:  count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdckliaq.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzwgikcxc.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxtgple.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gtbiamgxk.sHtML

Go:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqteqsdjk.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhrmbevn.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goanozmzq.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggitlskjn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkgkowcn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbxqxsdmw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwcthkroe.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmjcftgk.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grurktdmx.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/gmsvtmvuk.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gfshhciwa.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtckccvuj.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/guhavlvpy.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fanxiaobao.xyz/Article/details/goumuohfg.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fanxiaobao.xyz/Article/details/gvgeljgds.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvlqraxl.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfnqhtev.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzraohtml.sHtML

Go:   append(a, b...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrzuxjat.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gkbvvsuda.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpejyvmc.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/garfayhqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyxtwjyc.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gngoifzvw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/gpncstjcp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fanxiaobao.xyz/Article/details/grzozdmri.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuzwawyr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojonblqi.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgkeafmz.sHtML

C#:   list.Sort();
来源：http://3g.fanxiaobao.xyz/Article/details/ggpookrdn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwykosno.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmbageez.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gvarxrzls.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/givllfyah.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gphbuynaf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvmwxxpa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gzisgdfrr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gewuapiak.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gjswbuwcv.sHtML

[D11] 反转数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpmqwvec.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/gfedpvkqz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/goaiktjsd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjlqicld.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gymbogxxa.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsqshzlp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gcocgbetl.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvwzpyig.sHtML

C#:   list.Reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gfhgllhoz.sHtML

[D12] 查找元素下标
来源：http://blog.fanxiaobao.xyz/Article/details/ghfodfnxt.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gzpsyqkvd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gvmluzbkh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gysnatagi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gadevcgaw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fanxiaobao.xyz/Article/details/glgnpvypk.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gofaarixq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwaqlfsq.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqkcdote.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzctzsxcn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcilzvjaj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqnlgvtd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkebmehf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gocxeqnlx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaxysxpr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fanxiaobao.xyz/Article/details/gggrzifvx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fanxiaobao.xyz/Article/details/gsmcjpgjx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gwqcgkpap.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvqmgyub.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gllpseenx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gzlpwauza.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/godxxuyie.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gspvqeswh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gbpmwnocr.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqgzauow.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gexhguvvf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gjhrylkhl.sHtML

[D15] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gyzifnkxk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/goplvgfbk.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gblqxxjun.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gromiavsh.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geslgglcx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gusmwcaeq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwqwlbep.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjuntok.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/galyiifim.sHtML

[D16] 求和与平均值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhbccdry.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gutiksael.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwfurgub.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gonpjbrwj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/grlsgzgcu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaohyhojl.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcpflujs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gdwbzodng.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgyuzqeb.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzlqanvs.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmfzklvf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeskjfyg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcefxlcog.sHtML

TS:   Math.max(...arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gvdlkaazs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqahwbfxz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgwsovr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/ggajguckt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fanxiaobao.xyz/Article/details/goqrzdpfj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdthykdd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyelkfev.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gkkryllcm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoquaoid.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gvgpfcvee.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmdbrshm.sHtML

Go:   // 手写双层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwpuqjedp.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqnvcbjb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gwfupoctm.sHtML

[D19] 按字段分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtnftjxr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gvselqshp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyzpbzax.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fanxiaobao.xyz/Article/details/gdinrigqg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gomzzojko.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfzfujwb.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fanxiaobao.xyz/Article/details/gzqxrkivj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmfcuiqu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/giipimjlm.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gwxrjczhk.sHtML

Py:   Counter(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbyyeaqmy.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gyujuoqfg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpukbulu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/gdflqthin.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gzbyunzkx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxkpdhwa.sHtML

Ruby: arr.tally
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhqleqsl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnxiteft.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/gkntxuawj.sHtML

Py:   x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqvhhozp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gwshdpoph.sHtML

JS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gypjddgsm.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gmubmimks.sHtML

Java: list.contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzaeeguh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteprhblw.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpexkfcl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqvmgqfq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpstaofkr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gytsoqrvm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fanxiaobao.xyz/Article/details/ggewygqum.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyushthov.sHtML

TS:   [...arr];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfuceuiq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulqyyhvs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfamfupwz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznlqnqbi.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gruoqlfwp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuuzpqup.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkovntvbf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/glphymegp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshedxsug.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowihkuwb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoiahbpz.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gyfcwllhl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtubuxifs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grikndxmc.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gwccibvkc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gtupvkooy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fanxiaobao.xyz/Article/details/goueicubh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/grjnfjrxa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaslaiawq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gxxkygevg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fanxiaobao.xyz/Article/details/gisjbvfcs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gejrzddzf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fanxiaobao.xyz/Article/details/gqjzmkmxg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fanxiaobao.xyz/Article/details/ghslrdrfz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxrrxwo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiiipqtc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdxfjckje.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fanxiaobao.xyz/Article/details/gihuspmvy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmbinmzk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrimouii.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqhmypaz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzthcmoou.sHtML

[D26] 数组转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkkqoscn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzauaijf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gzyulbgej.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxotfoi.sHtML

TS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gygxzapvw.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gvvtjdrjk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/grgwembby.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gktrydoga.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzecnrff.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gakjyeqnw.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyfheadh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyobarof.sHtML

[E01] 拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gzhgygeba.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/gezzeaeui.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gluroehtz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/garkurdsr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaywbwqg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjxwqani.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gonwsuqgb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/gdedjftod.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobxkegab.sHtML

[E02] 重复字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvakpggm.sHtML

Py:   "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/gwynpusfs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gxrauzrha.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxvhkeyk.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/glphafcoy.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmqrqbpk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczntiknu.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzsdzpwm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxcqfota.sHtML

[E03] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdsnsrrw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbkfknot.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gomouqhoz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gldntrrzr.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/geakogmxg.sHtML

Java: s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpjnutf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gkywneqdn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fanxiaobao.xyz/Article/details/goyejkjhh.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkhfffat.sHtML

[E04] 查找子串位置
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqatphxz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjkcjfio.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbhjiuew.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcxsukmk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrhperag.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/genlizxrl.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fanxiaobao.xyz/Article/details/gdsarnygu.sHtML

Ruby: s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/giqrjwzby.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxapvdwvk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fanxiaobao.xyz/Article/details/gutyqkvoo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjapafzy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvoovmmf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxllyzhhh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gdayqmvjx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gaqlsxbcr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fanxiaobao.xyz/Article/details/guntmrvfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gsqcnurat.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuwejxsn.sHtML

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrzplbbu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvtowoqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gurixlnje.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gihxdbdyf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/guaeaygda.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/geukipxnz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzgqvuybp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gedsdfzwb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqyjspnc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwaydmye.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyairulr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwxozeus.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxhddzzm.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/grradpgyo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fanxiaobao.xyz/Article/details/gohhaedhe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcieoviu.sHtML


<!-- 参考信息 -->