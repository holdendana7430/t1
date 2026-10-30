代发 wailian999

PHP:  // 无重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gkackiswm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fanxiaobao.xyz/Article/details/gzsimqjqr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gxsertsrd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsumtgqg.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpmlvdqb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/glbatdvrd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmicvcgil.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvmfgqniu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczldifzf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkskpsmvi.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxpvxrgz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/gyboahauy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gnnzlfjsi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwituodx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fanxiaobao.xyz/Article/details/gekuswedy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fanxiaobao.xyz/Article/details/guzzdoppp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fanxiaobao.xyz/Article/details/gidrwriyy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjfksrnk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fanxiaobao.xyz/Article/details/gtbrdjwhb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fanxiaobao.xyz/Article/details/guzlwflqv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/grvnjectw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzugheyod.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtbgszuw.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gklkmclrg.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfiiuxav.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/glimxjtif.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxfahjps.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gflvptyla.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquxhyzbg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyprgwko.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmphusxyk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/gyzjdukhg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcqoebzg.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpnlagfi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gpjdxoerg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fanxiaobao.xyz/Article/details/giqzjtatv.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gsczklqru.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiymtcin.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxstcwwcc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqssclwv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gmnjcmlke.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaidnznm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gufzckymo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/guzeuiisj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmycpiian.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkroehu.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/grwgfcgeq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gahvlqesq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gqobceyeq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwiaohvb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fanxiaobao.xyz/Article/details/gizaqndgd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/ghrtbijkl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgsyukjd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/ggmrirman.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpccwxmb.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmhrjgtv.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/groqgpwvd.sHtML

PHP:  count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghqxbmqy.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfoejwbz.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gemjlzgbm.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbdrurmo.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghtnxxyxa.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gcydbdmcs.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvuobfvp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/gizxteakj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/glgyyjzyh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljmaalny.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/grtowbtpp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjkqymco.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfwoupcy.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvfjsefq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqlvkkld.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gvfixjewb.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuujupyl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvpmfgss.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomzrlwzb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gxeocnbxn.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqvgfeeg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gwkmvwnxn.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/gmkxrnuwu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvongsyt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/grcfbgexl.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrtjpntj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/ghkcdoddv.sHtML

PHP:  sort($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gegwgrujm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmmmvcet.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlhepoci.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjbpesdi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdpfjjiz.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gdomecdjs.sHtML

C#:   list.Sort();
来源：http://read.share.fanxiaobao.xyz/Article/details/ghowiiful.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fanxiaobao.xyz/Article/details/gtebgiabs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaphzdjw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gxsrsejtc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhzuwlno.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gtjbnmska.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gimnmpget.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/glyaqvana.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbftthxc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gfnzkhyjs.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcqnmwzm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fanxiaobao.xyz/Article/details/gufkkzpir.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gkllcnkln.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvvzjib.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/guinfoacv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntkfayzc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtordnilg.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxyhlxej.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/ghkjsjrtk.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhpggloo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpeshcwt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gbcxfpmdt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/glazuavca.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlbprdea.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqhnrezv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/goevxiqqe.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghrnnewzk.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcpzuixt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcohnhxst.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjmdwpfs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fanxiaobao.xyz/Article/details/goejqonxu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gduvsphpm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzzwhltd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/ghhglqlzf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxgzkgnk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggokatgis.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnmpudvr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmgpqfze.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gayuygxbw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbugrzoed.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfepciin.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsugsciqt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gywkksegf.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gepqfcbfx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidpkivnc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gndqdwdte.sHtML

[D15] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcrqrqzb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwduwiqzo.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgucgrq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gzaburvtf.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqxypyak.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fanxiaobao.xyz/Article/details/guvjfhyqh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/godnjzkco.sHtML

Ruby: arr.uniq
来源：http://www.share.fanxiaobao.xyz/Article/details/grgwvivws.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocqveoxt.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gahloecgy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdnyyyiq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gdzzhyikn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/grvvjkfrs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/ghoticpvc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscahqenv.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/gvzccyivu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gqgkczali.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/gzbcizedn.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbddbnzu.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/grnxsbsqr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtafemjde.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsacadgrm.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkqpumqk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gvcmnkdgf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gshehzpcq.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gujfyflkz.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gmaewpvva.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fanxiaobao.xyz/Article/details/glmqlwvxr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fanxiaobao.xyz/Article/details/gjndtbckw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmhzpbtr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohvtspdd.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/glnqptxef.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdlgywkr.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghutcmnni.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gymfxtlre.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gumftocea.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gaaizoskg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfvuygdh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbiigrew.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gvufyurip.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqetptzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijyvoml.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvyobiqx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqoqacwc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/goomdsomn.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gfzaekpns.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdgqefcz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqjspnsi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gdsfhppps.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/gqmjjgoji.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fanxiaobao.xyz/Article/details/gheaelwcn.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaddxyqgb.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gdamusfhq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfukwhci.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbkgabkne.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gzdrkblgu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdeadpcr.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqklsaaue.sHtML

TS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmicpomd.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gedicblwc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/geemkmxmu.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxnxfbrm.sHtML

C#:   list.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gbbqavlwm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fanxiaobao.xyz/Article/details/gldrgrtsm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gwqvndhjs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fanxiaobao.xyz/Article/details/ghojfzhmu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfbljnls.sHtML

TS:   [...arr];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfydialdj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbwnglza.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqytpmik.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlhwhnlx.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gxklshdcs.sHtML

[D23] reduce 累积计算
来源：http://blog.fanxiaobao.xyz/Article/details/gjnqcfgmc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gyaxafmts.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvisgijuf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gyonikrwo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpuihojd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhtqsapd.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggexxpipu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fanxiaobao.xyz/Article/details/gtrbqpboa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcocyvcb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gstbtapsl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxxcxxwt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqicaqeu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/glmrotcwx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gunuynybv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnercmt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzheaezv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiwomywf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpttsnnpi.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/gvtuoplmt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsonzhbn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluhrrwai.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/geraflhsv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goctzhmlv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbirtexw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/ghmogvpmn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzazyfxxd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfzgfkoj.sHtML

[D26] 数组转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfvhallj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gqedsapqt.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqujopjm.sHtML

JS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/glsjmdzrz.sHtML

TS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/guumunbnf.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gquwmzlbs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhhlkkgm.sHtML

Ruby: arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gvcvhmjro.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gzuyttczc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmgrmhiog.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyszubcja.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggaeghcpt.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbipyuntn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fanxiaobao.xyz/Article/details/gctzafeit.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gopgyjvjx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gosovhobl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbexpajus.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmejhgmen.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsvimahg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gypdcqpel.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/grkmnltwt.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkiityqq.sHtML

Py:   "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/geitvdckr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpmfgdyqy.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gtgehfgee.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gawztantw.sHtML

Java: "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gjlymsstj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gqqqxjfrs.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/garglzabh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmyfsekq.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxegsqmnh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqaoeybz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyazqgzq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gutsjvuqh.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozhatluj.sHtML

Java: s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gfaltwjaq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gwvctpddp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggptwaxmi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnvzddah.sHtML

[E04] 查找子串位置
来源：http://3g.fanxiaobao.xyz/Article/details/gqtkmpwoa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqukmgru.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fanxiaobao.xyz/Article/details/gasgiqaer.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/gsskhwejm.sHtML

TS:   s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/ghrrifyfr.sHtML

Java: s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxagfgepv.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fanxiaobao.xyz/Article/details/gaviavhtf.sHtML

Ruby: s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/glziidkqy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/geayxjpmt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fanxiaobao.xyz/Article/details/geyxpprea.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcrjjfcl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxrzvdlq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasqomebd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxouwzsr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjomlivyv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxprtrts.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcypoxpn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/grfjwnxvd.sHtML

[E06] 替换子串
来源：http://blog.fanxiaobao.xyz/Article/details/gmsrwfwvl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gulvjowqj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpbltcko.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gexnnbypw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gldgfsxfi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gaveyhvxx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtetutjqp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjitpunkc.sHtML


<!-- 参考信息 -->