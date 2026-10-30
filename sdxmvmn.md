代发 wailian999

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gxathyjxq.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gcjjjgzym.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/grftemkmz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gwrhbhtam.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gvzdovocw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/ghjpdohmu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gvhcmstyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjpfavqxb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gomimyapj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/ggckpjcqi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gntspjmso.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbhnhuezg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gzlwneprm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcitxqhwo.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gtyehzcvs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/grlhcvspb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gudoczvbb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/grjhcemkv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gcciwwrlh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gytmblgfg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/grmdofbvx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gylgzjmqi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gvayptfpi.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gajbosljm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/ggjfpgbnm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gfggmgsnc.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gsopvktow.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gjalztczj.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gxvzbpxxu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gpafggovf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gnajocoau.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gtitqatpo.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gnvabetdb.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gjclccoqy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gknnmjpsm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gexrzhecj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghqbegnfa.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gtwririne.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gzvrxdhtn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gxyvaidyg.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gwzwldrej.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gjeatexev.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gufpolwov.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gbuhsqtfi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gjecrhxty.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gbbwlwrqe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/grurbyuzo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gxcspaeqr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/ggywupiqg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/ggxyryvdb.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gjtbziint.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gfqyzjgjh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/galschwgr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/giircckig.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gemoquzfp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/grsqxpdjb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gcioepbtr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gomntasdi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gofsgbbig.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gphdpaxmf.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gshrowodc.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gdkqobnba.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gctakncvi.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gkcezpcxn.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gwizdoqgs.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/geourooef.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gvnqtxjvu.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gjcphrusz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gfshuyiqq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gltjhazgh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gtgpizaeq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gbgajkppt.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gfvleodzz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gimatdexc.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gvffonlid.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gnhjeacpf.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gospjinsj.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gzuuchbgx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gackgxfzs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gibjuefls.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gtxafcxxy.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/guuqbbbyg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/givlqmotr.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/goszxxwbz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/goqpshgll.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gliumauax.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gbhsmepgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gcqoowolt.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gvixhzbpw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gdzehzzii.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gehekevtf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gacsomiyl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gezqzxxdi.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gprfffhch.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/griodkanv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gaprzvryv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gzfwuyjmy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gzzeqcctf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gidkcjaoq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gnafkbavl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gpyympyow.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gsmevfwnm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/ghkhidhmq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gmfsjjwps.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gksoujhsr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gbeswlpxb.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmyriie.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gopvuynxn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gmkgdpqxd.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gyzzcemhx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsrhsvkfi.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbvbtphak.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gwwpgtjuq.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/griisxfdy.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/ggkppetiu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gcmjnzxha.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gupojyqii.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gvbggsgdl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gapyixweu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpjloimjp.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmvnwjnsj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/glkanyzsh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gzehkdnwx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grojsirzo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gxozjstry.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/ginaquith.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmqmjdfor.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gytbzlljv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gmibzgtte.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gnvqkhsev.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gqngydcmu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gurhttuio.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gkcuswfit.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbumzkdsm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gygdblibl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkcvddfrf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gceovwwgu.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gmzvqmvut.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gzltdxeki.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfuiuiom.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gnwdashut.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpevbhinl.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/guowmvffk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/guacurxdc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gyzghbhmq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/garqyfjww.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gmriixxky.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gkhoycteq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gboiknwhy.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/guzisrvqw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gdowhsido.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvwapbsof.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbdrflmth.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/grweckxcq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gwenwpipr.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gyttaewpd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gmspmembx.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/glbomxxlv.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/ghtohpuyt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmrbsyozq.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/ghkvgcoqd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gpsssacjt.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/ggbhroijh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gdyvofiie.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gfaqmqzlz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gnpxdufkt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gwetuzbnt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gycwwviti.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gwjpjpkan.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ggibwsciy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/giewdwskx.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gsxfenfnz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gisqcyaaa.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gqhbytocb.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gouqlgjza.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/glfjkimeh.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/glppwqjxm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gacxgycvb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gfsthojeh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gfobmlpyz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gntlpwfgy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gletkgmqh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gpuarwntc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gbpfrejuc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gyubbncdr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gxfzquwim.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gcjfwhyou.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/guhthjdvj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gzxtpkkob.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gcyfxdifa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gislpdqac.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gtwrmyeml.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gfguhbkuk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gkudwrpbt.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/guztrybni.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/grlnyprbx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gtfkbfizs.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gdqwsanql.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gjelunwbo.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gueagydsn.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwmxarlvl.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gnalifflf.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfflqttom.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gjftnfmcr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gknnjcfqq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gwwxhrmsj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gafxjzooc.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gwbfggqst.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gowhzhkgn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gdisfzown.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gqzjexwvp.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gbcqbddfg.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gsvgqepbr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gtcrvtzpm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/grldqbhuw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gmpjnezfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gkrojbkmo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gynuruovh.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gtbaguueh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gbpixtnbx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gkauphbrr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gbqsveubd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gyudjocyf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gyixclzqf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/getbtqsdf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjnoqrxqk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gsnbldzlr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gppgudvba.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gdscrpwhs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gilmochdh.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gqdkkohsn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gbhaemrrj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gfnkhlftd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gevylnjod.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gejlczsax.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gwaoldenj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/grvydjerk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gfbszijzg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/guvhqxqyk.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/glxcolwnf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gvzzefqgl.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gbilkfady.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghyoyetyr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gferkobqa.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gaynbuwmq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gybvdpaak.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gdopmqbbt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/godqutpbg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guldtttnw.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gaowjmnyu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfrvrmdtm.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqvvbzugq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gdzggokmb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gaayuasvl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gaoamxcsm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gnzirdpmn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gqnpqaoaa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gmeuihtuc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/ghdjswxsz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/giicnkrgl.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gyncgzlxu.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/ghxyxzxnc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gvotqbuvq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gczgwtzlo.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gornmpyqu.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gmkmvikcn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjddzoeas.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/grjuutudr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/giypoiiem.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gymhqisft.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/geczvkjns.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gfdzuiivx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gtlcgbbqy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gfluhjqme.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkuojdpnm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gzlzkyxlk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gfkmnwtwf.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gicbzoxvu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gnthxxaqh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gsagrpnsv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gpofgbhjz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gguxjxzou.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gyzdygdgv.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/guenrrabk.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gpawglcmy.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gdppbqanc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gbnwnqvey.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gwxmbhfuh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gwrgmrguk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gswkaogpe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/graiyllna.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gvrlozhhx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gbrccfpek.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gysvffupl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gksjiesum.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gurqaomdc.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/ghgbqpgeq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gstyhdjpj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/ghxptnmzy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqldqvshp.sHtML


<!-- 参考信息 -->