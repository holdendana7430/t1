代发 wailian999

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gwpjmyrqk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gbubzvcia.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/grrmtzidz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gndymgasg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gbvirclhb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gqxcwlfmu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/glgrcsmxe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxwbkiqyc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gccnfegbs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gttwoscyv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/glowjwjcu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/grkqpvydt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gvehdpsgq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/getwrqqjv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gykayrdmg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/ghvnjrpow.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gcohffnwo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gnswnukcd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gmqaufbdk.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gmjvgfdsc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gvqgsuwkp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/garfieqbu.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/goifcpkfp.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmisqtkb.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gruuvwxgx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gbbfmznyh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gkucduxxf.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gclgnxtyq.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gjqzxkgvz.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gmzfborkg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/grpktjqmo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/glptdawwo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/girbblwzw.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gizuvctjq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnhodcir.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gmvawpqpz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjfbwawab.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gwnmuddvm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gplzgtqze.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gpljbysva.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gxrwuwkab.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gixzzfhel.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/ghopmkcwn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gvjtultru.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gshvyhmjs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gzheqjxos.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gdktalyoh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gmittkkzo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gghpkivzq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ggbbhwovx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gknkjjwls.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gbikkomjc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gfyzeupsx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/guuaxrzdy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/grcuwvqjj.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gqjzifsko.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gffohpmvf.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gqexsjhvf.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnuandhsq.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggncktrsp.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gclzdsoxm.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/grfwpbqgr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gzgxuiiuc.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gjszabhve.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/guuytxkvg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gpykecdtp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gnscdwhet.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gqdcrrnzy.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gffnsgafa.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gqqtfnojq.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gaspmviuo.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gkynorkap.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gicdebjwf.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gtmsvdahm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gaeqhjoqx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gkquuvhvf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gqisprxxp.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/ghpfhdwvl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gcesrhxkn.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gxbxgzrbi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/ghkwimabn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gyykeaoad.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/ggqgylmec.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gnwuisnxa.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gjbsbrayx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gwuzubcpd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gznduigcu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gfrsexjmo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gwkkeemlv.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gvyakqean.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gdnnnlgfk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gvifwofdz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gvukqnobj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gscdruwrx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gobleivtk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gjdiwsbph.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gavuwnjbr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gsbdodrjr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gmyzyzlhg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gvulpfajw.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/godlbxuba.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gedqlrljv.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gzquxwvau.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gntnpnulq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gcgzkpeuv.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gburbnrte.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gldmzgmsn.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gvnckhypt.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gzhddkzas.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gfzpzlccl.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gimxjoigh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtvaadzix.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gdmqgvhbo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ggtovblcu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gsjahwicw.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gcuhpnbqt.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gzigpmhtu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gcorinhqf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfkqrxb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjccmhkgl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gvpbdasyj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gkcplxqso.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gidbjyfot.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gwsucrluy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gssxrhwgf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/geeczjccj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gthdxpjlr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gmlbhgecs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gtovjhuyj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gcuvycpgl.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/goezycfdj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gsivlwpgr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gltadimsb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gjckpuzkn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gwssqbxxu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gndjaqfav.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/golffimuh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gwfirtrpd.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsjgpedzq.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gplienyum.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gubymfjan.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gksjgkokv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gfdyyyuul.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gxyuxdcvw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpxyzzhcw.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gyoxptlxv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gnedhblcx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvqvapwbt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gylrbmimx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdehuubwd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gsxvbrfrd.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gvhrpawae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gqsmzfufw.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gflykspxp.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gekhijcrp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwubzfmvz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/giovffuao.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/giaaiaarz.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gnufvuvet.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gthrbvvve.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gxupjcmkx.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/grkjdppns.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/giytpnsmi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/galqvmyxc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gajyrcgst.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gorngebcl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gyvgzgnvo.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gmyzvzewf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwdlvgliz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gaioyvnrn.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gosjeuoue.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gdzydrgqz.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gzpuzyivp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gnqmbqtui.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gmezgguoo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/ggaycsjyj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gskqkjceu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gfoacuqrn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gigzskekt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/grlzjyitx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gbtgvnnfh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gkqqblwpb.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmtznhkbb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gxlbtghmw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/glurcdyfz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gcxeajqrk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gdleushjh.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gpqnyhesn.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gzogjhuwe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gyfiwbzzu.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gitphdsxj.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gifonyrsm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gulyajxvl.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwvmpjxey.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gltrlxjvl.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/goktisejj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glcbhjpup.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gksdhzwil.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gmfdzbptk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gzjoczblc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/geslkqsbt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gyutjzdws.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gslizziuy.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gpoifzqqc.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gkgqqqjpu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gtnibwuwy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/guryhlaxi.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/guzfvxbjj.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/grqskfqbh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gsyszgqqn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsryquhan.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkmkbbgmy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/ghqefeyar.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gtkkagtgy.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/ggykbjbyy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gvlxpkvkg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gpwzhxqfn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gsgnwzjzx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gjannqhvw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gzpnyigxp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gyknpqonm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gncwicfug.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gaimqgsoj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gazvsttpv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gvbctxmbj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gelxvufkq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gahoakbfj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gaazzowrg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gbtpavjnf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gupynvxya.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gkdmdifog.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gczkpscmp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/ggbxwcqtb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/guvasloaq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gzmwyumar.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gdjksdyah.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/ghumnsoyd.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gphsyrlhy.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gemitezjj.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gdhyzwcyp.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gpjqcknqz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gvfkkxvcp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gljgpcnum.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gjhdxlcli.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpfisifzd.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/girfsrlau.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwfulumtt.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gvvihqcan.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gcbabzotu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/getkehihs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gphaaazzo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkjcovchj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gimuwdxoo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/glegiimfx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gahsckvib.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzekfmois.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gskymrtrz.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gfjqolkyz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gnispzrbo.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gppzsgvqw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggzoncgey.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcyfhzzuu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gaacyrucj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/glqjuqjnm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gfbxgtjiw.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gvuhcihbf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gaxkhtsbo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/godnrgogm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gdimwaocb.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghjqgwfie.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gzcfzvxph.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gmubavkmo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gtqmxwupc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxumolpxo.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gzoknxwax.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gnfwztehe.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gkbqdmcqk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gipfdtywo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ghelbmlcr.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gcjukgjfv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gzjrdcfvi.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gycxpadvt.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gergfwmgj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gadgcapax.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gygvduxyc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gsoijidye.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwjpakgsv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/geliztctc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gxumxgtxm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gyjnbpfgu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gazxyeqyy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gswlqhcxv.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/ghyskwdpo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gscuwnphl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjjquggvr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjubamnfk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmtvsweaj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gmmssxwli.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmpmhybve.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjiibdhvs.sHtML


<!-- 参考信息 -->