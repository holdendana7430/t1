代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqwjdngq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxfdhdrfn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gswwdndok.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gchxyharj.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gzztcyeqk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grduznxlp.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gbyupizki.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gypsctagr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhzxenmo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcbhdnlv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fanxiaobao.xyz/Article/details/gusmskoud.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fanxiaobao.xyz/Article/details/gdytckyuv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrksalfs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxyounbi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gutzqvrfa.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gejiboruf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/glfacgoqo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fanxiaobao.xyz/Article/details/gyirskicf.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbaijqcc.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gnjmsephc.sHtML

Java: list.add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqnnimx.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlcammbh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzgwzmpq.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvmkhzvfm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grbctvuto.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gaelbwksb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnwyltswd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fanxiaobao.xyz/Article/details/gcdncupax.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/geibywipi.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goklqutca.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamxnkotj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/glelokmfe.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gzvicyzlg.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfbotlr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gexmsxcgd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gptocygor.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwoifgdd.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gcdcvzrcw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtchogghr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmmqmhpx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/grwkmyrkg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvapnabwz.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzhnmdve.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gpngwgyqp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwohyeqqz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbboynsmv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdqlfhie.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gsshnjqxq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqktmnwfh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gvxinhijv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisdvoade.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvncflwql.sHtML

Py:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlrfmwor.sHtML

PHP:  count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmynvwmc.sHtML

JS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/gyrjoqnjb.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggffyjqoh.sHtML

Java: list.size();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnqpiyrr.sHtML

Go:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmvvujjcb.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gspxfoxqy.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckbhtjjr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fanxiaobao.xyz/Article/details/giwbfberk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grniftozn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwptfdu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdifnghp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwatklsg.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gylulugxi.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/goudyisyw.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gvowadies.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsdkqtzj.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesqwyco.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gldlfympw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbimaast.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gguhnvrut.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgelhxml.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gneombpdx.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/guwdotcqt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfvdgney.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwxknxzg.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/gpjpvsqgy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdsdqlnz.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gcssshzdz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fanxiaobao.xyz/Article/details/gqxgubjuy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fanxiaobao.xyz/Article/details/ghogsypdz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fanxiaobao.xyz/Article/details/gzongrmnv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gdxzhxdtr.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmeaarql.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbolkmlc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnhlaafr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcrbigxn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgqqeblz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gaqukniug.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnepfolbt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gpxfcaass.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/gustodtti.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqowckms.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gdllhoosb.sHtML

[D11] 反转数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gopjabudd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/gmcaefpdu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/glwhjgzjt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gmpkgpizg.sHtML

TS:   [...arr].reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gdmjmjaqa.sHtML

Java: Collections.reverse(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gerzbzcub.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrvrhgvx.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvaklfbt.sHtML

C#:   list.Reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqpzyyep.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gxryanqbr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsaoqhge.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/glxtakzvk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/glxorzodb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/glbukmssf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fanxiaobao.xyz/Article/details/giployxwc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmomljxbg.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxlygcrso.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fanxiaobao.xyz/Article/details/gxykhwgbj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiipzvvz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/guovsxfvk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjouaqhn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxpopejy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giugxkcgt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/giubpeuih.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gppbpuqbr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/geklobexs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/grdduvmlw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gqumhjhcf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxbducft.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/ghhjystxl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdechysbl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gumxfrsow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gqhjrgnms.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gwrbbmgei.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gpaptyffc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gktivbdnx.sHtML

[D15] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/geqdqqabh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrcczcfv.sHtML

PHP:  array_unique($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/geqynemyy.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gzveraydd.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwujptncx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfxjgfcs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfzbqqyx.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/gxuznujgd.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/ghyzvrbrb.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzxjbccp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfnmejzs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoynbsni.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzmshtxc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrlnmljx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fanxiaobao.xyz/Article/details/gopmqmbkc.sHtML

Go:   // 手写循环累加
来源：http://baike.fanxiaobao.xyz/Article/details/gtylnumvd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhptpzzh.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/gubbuwcas.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqpwkqsu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaixyklm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gvsddosqp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwrzzhhw.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/glrjscnqp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gotpwfmhu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnlnuopp.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fanxiaobao.xyz/Article/details/gvnjoeyht.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fanxiaobao.xyz/Article/details/gzrnzxqru.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxycfanu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gozwmoobn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/gotxnuiap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fanxiaobao.xyz/Article/details/gwsrvydyn.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhtfpuig.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/giwjqcwmo.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/grgimvojg.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/guwufofca.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdrbvmgl.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdchdgtx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjalkeobh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fanxiaobao.xyz/Article/details/gfvqkrlmh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fanxiaobao.xyz/Article/details/gtljfcizt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiiaygoz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtwcobve.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fanxiaobao.xyz/Article/details/gtpjtiohu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpoejqib.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/gougpvkxy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxqnxuye.sHtML

Py:   Counter(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gdllbqvns.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitpyadyy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gippjvwbn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/guftoqsua.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqyosoqt.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fanxiaobao.xyz/Article/details/gznsiluet.sHtML

Ruby: arr.tally
来源：http://www.share.fanxiaobao.xyz/Article/details/gbheumptj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/gcbbjxqsv.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrxzybgs.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gelovhzof.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpglagecv.sHtML

JS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshlfpypq.sHtML

TS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gumspswjd.sHtML

Java: list.contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsrjdltv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkuhtcvkw.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/goucznoob.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqtgbnid.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxkmpgji.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gftuawgan.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvafyrvi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gjvlzycgl.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlzludng.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gronmcghu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvyxtexr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fanxiaobao.xyz/Article/details/gfmbkgaih.sHtML

C#:   new List<int>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaehhohz.sHtML

[D23] reduce 累积计算
来源：http://read.share.fanxiaobao.xyz/Article/details/gssapbxfp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxowuhfhn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/girypnhzc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/glejnprbt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpgztdgo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbysmgyde.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtoxgewne.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpyofkff.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghprkrdnb.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fanxiaobao.xyz/Article/details/gzgvjygyt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gxgsbbeno.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gayjttaax.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnajkbtcg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gyqdyxqtc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gaheylgol.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fanxiaobao.xyz/Article/details/guyibfklb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gsibarajs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidoglfru.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fanxiaobao.xyz/Article/details/gglcxgoxq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbvkyhcs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gscycahaz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqyjfezb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqylgjrib.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqoxclfj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gmnqjbsrt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gggdrfqiz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxrqllv.sHtML

[D26] 数组转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiwcckqx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdkncxct.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gjviajowz.sHtML

JS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gboeaadil.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gxlbqnoqa.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdtbovis.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gobbjiseg.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzumpuprq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gysgyifns.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnurblhkg.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gknuhkuos.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grlmzqfrp.sHtML

[E01] 拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfniixznq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fanxiaobao.xyz/Article/details/gxffoclgk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gkdqlhhlf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdprbhkd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxajopbkj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/grgsmlhsq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/glrlphyoy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fanxiaobao.xyz/Article/details/gufwywhke.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxarvbcfh.sHtML

[E02] 重复字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdgoafnzq.sHtML

Py:   "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/grijdkfow.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyekezsle.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjnfhhx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwosnrkoa.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzyetcwvc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqipmmk.sHtML

Ruby: "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/grkpwkvva.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gaderypbz.sHtML

[E03] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gldewikdd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbumrjbd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gmsnjyboq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gqmrftyym.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gtwzlmpta.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsuybgux.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklnwsfhi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnwfpiaf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfexfkvuo.sHtML

[E04] 查找子串位置
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdgdvpm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbawlfcom.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fanxiaobao.xyz/Article/details/gttnmlcqp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmrjsekl.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqlrzdss.sHtML

Java: s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwhqvwhv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/gctzgmrlx.sHtML

Ruby: s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxsbxyoo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmoolpmg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkucqdxfu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcddvwtsu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkdnanss.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/ghoojpoaf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeydnodb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlbfzifd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/glootlzst.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmpjkoyq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwdstgtr.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/gakyymxwz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoxsfugg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkzbvrmj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gahmukgld.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekbwekqy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvhfvxly.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucrjlhde.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gjopsayks.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvvdnesi.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gjsvcqkdf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fanxiaobao.xyz/Article/details/gjdjismfe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gcoewnxgc.sHtML


<!-- 参考信息 -->