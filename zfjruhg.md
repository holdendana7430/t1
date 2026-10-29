代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gwvvzbrdk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gzugtjveo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gstkkqdkn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaxpywvje.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gqovsiece.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjgwwotdw.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gxynkkivz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gmwmgibcr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gimokhpnc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gtnopasjq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gdcbzceej.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gksgzpaee.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gpxwhsggm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/ggnhxguoo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gptzafwmf.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gawixcmle.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gewqhagwc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gwlufkfkt.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gtyxgzquc.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gqkmeiueb.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gfboyfjwq.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/goxqesfag.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/grmrfspxb.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gmllvuayr.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/ggqexdbjm.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gnbchjsvj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gkqcakfyg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gcazmbofx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/ggrvpznqj.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gxuspasju.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gzwenihtr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gqugplajg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxefvzyaf.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/ghjeytxly.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gxqxbjmni.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gkpnpwhta.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/goaxifmja.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gfctbkvjs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gfgknxffg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/geugxhzqb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gmsufalda.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gmabkdqja.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gceyghqvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gryfsbodw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gtoipmmax.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmxfyqvip.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gfveulpxt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gvjvgtjde.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/getzqyjcj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gqlwwnuev.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gvxctfetp.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gwybxzhqm.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpgrsrbxk.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwwnjhxdm.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gmxhppsgu.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvryhipkl.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/geefxyufc.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ghbjalcsr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gobxszqkg.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gxctadzpx.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gqmlwbwal.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gapogthnc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/goesycntq.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gkoafvobd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gthyvvgvh.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ggkktcqun.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gafqdyzcy.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gcqaykebr.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbwudqozf.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gkcayixtg.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gfgmfomtf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/giczrtosu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gzwxvkofz.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gykegjmfr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gtnwviepf.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gckrvbpgd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gotoaiijq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gcjiyrzuh.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gruytxdtl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gcbdklrzh.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/guaucoljr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gwdbyinxt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/glieoplxi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gtjnshpaf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gkzwqkmzj.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwpevixdi.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gyewguzgl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gapuzxeiy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqphibcp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/geyrmjhgi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gjexdrbhb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gumuluoiw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/grggdxciv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/grcsrhhfd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gtsffsmju.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/getzuhdxx.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gxenpocwe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gaumkzija.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gxnuioypa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gvxpxcdgo.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gxilzlhcv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfilyedbv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gpcknqwbo.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gxeycxcix.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gxkyqteed.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gylxnneys.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gnvcryaqv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gpsvmwnjb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gnxkkbusx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/griejktqj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gocprihao.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glzekjptq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvsqozuzj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gnjooupys.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gpkvrphma.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gwhgtytcp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gewbdyeuv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/goabupolh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/grpafunba.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gobhlnhqw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gybqkybdw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/ghihrdlvr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gxxandooa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gzhfihwqv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/ggfsvylzi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gulustlqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gsenglguu.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gmbsppzod.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gunlgonbd.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gajqdcvsm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gstgoeqas.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gyfaofyoo.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gtduccyfi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gjuzliduk.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gesbuxsow.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gdxtzizfm.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gszmwtndl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gcaacvjuy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/ghrevhsep.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gmklnydwi.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/girwkpmss.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gjxhiptjs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gnjypzrbv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/glycktdut.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvqfgwyjm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gjfyjomas.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gncnqelni.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/ggmjzompy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gxrhaqcea.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gxyhldkzf.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gehlbyjgx.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gtarpptow.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guvduginq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gfahuhebj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvdjjpnol.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gmjtqhlzj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/guuizxgfd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/goceflxgb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/geenmunlw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/grehgmwpr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gzobheyiz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gckyflnrq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gjkmtckkd.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gmxzeqlur.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwdjkssdn.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gfgrzfvll.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gfbrrpszx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gygorwycu.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/garfuaihg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gxxlbpwft.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gwydlveco.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/goadopaxl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gmiowbavs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gyenbtkjp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gaubtdirb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gbroseetk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gldiaetfk.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gxwywxekf.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/guzdfbzev.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gmxwdiujf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/geseqprgn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ggfpxwcgh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gjzemjzae.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gfejbhspr.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gsknlgunx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gdewlsndf.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gbhraayfk.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gmelymjsq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gfzgkumph.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gmkkdkran.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gqeynrklh.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/godvusclf.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gaoerxbrf.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gyerohtfz.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gyizzvouf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gfdrwfhkx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/ghhcigplm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gxlpyuvek.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/geaxdfvch.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gjulkzzci.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/ghjswjujq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gssnuquch.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gbaelbdjv.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gmqahlpsb.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gegddovpx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gpqatnjyz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwfxsyoy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gakjilyop.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/goacanrfx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gydddkbix.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhfeuor.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/glabigsaz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gbgdrxrkd.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gpobfnxcv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gyluyqfhp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gcznpltuy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqygzzrcr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdochssnq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gvcitbckb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gtpvzlecu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gvsbortsq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gtzkwjbut.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gzobwddra.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gyoptadrk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gtelkwadp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gqrnyyytp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/guuhubsfd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gopxedanv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gvbaxulfj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gdqmhzxld.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gknpmnohv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzfbyej.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gqmfhoenf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gszjsyrmu.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gzallffhn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghgqofhtf.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/guflfnreg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gwjetkheg.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gbxccohke.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gtoqdnfve.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gehrrnbhf.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gxgdxbhcq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwmlvdhkh.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdydggada.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gqxksdcwn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gtptahntm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gehuwsype.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gihkcmhbo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gykmvzfjy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/goypctrih.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gsimtbvhe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/grdbiehcb.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gjovtxmee.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ghmgtfdhu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gaqocrvrz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gspmmcjtk.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gsbddldmy.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gworxcluc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gydckhgso.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gqcrenjfl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gdkzbdfrf.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gdxzghgoh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gqnzkchoq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gxdzjzyea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gswnvyokk.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/grgpgsvsi.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gcfawhajs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/ggfmthfil.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gsqmeecgf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/goftlcmpn.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gztflilsg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/glqpsvkrd.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/ggjyzkmgx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gcnbpqzjb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghswvdprn.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/glmqohzmp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gczeuqjad.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmaecnfsq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gelnaxrhh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gbgrpcgom.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gufdaftwy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/guizfhsbm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gyjhodjjz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gxfdpyvnt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gzoynnyyc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/grkrnwetv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/grtcetcmv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/grqtdgozs.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gnsuhjvcu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gjynazpms.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gkgrxwqdc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gsxvowlhc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gkwgyfpra.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggboiapnw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/grxmnlhlv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/guwewidwe.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghnpvuzey.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gatkvqgbk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gdgbxghmq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjlpqyut.sHtML


<!-- 参考信息 -->