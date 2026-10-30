代发 wailian999

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gnnlyemku.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gqbqvqzyj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gloeaqpiq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gexablhcd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/giyctkshm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/ggfrcreay.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/ghfcyaomi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/getwashto.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gmdhvfhug.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goxsrlbui.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gxriudnvp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gosjsnaoe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gkjdxgytu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gvsyrftfp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gfmpkalpi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gtlehuuix.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gwkmkmmnm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gcpwmqvzy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gqohpegpf.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gpitybtvl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gafyjhakt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/goknwkkoq.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gtyvvrcig.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gcduggwba.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gyjgvnnso.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gispijkpl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/glmrlwngp.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/goboednac.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gxceutmhr.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/glaxomwzu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gkzjwpkwe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/ghappvdng.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gkwihpxxh.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gtpsjyhcy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gxpgwbumh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gscelrnnl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/glfcmgjbl.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gjxuncovs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gfwuyutdk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gdnqrbore.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gzsakzaun.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gomiclecc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gvgxrbodc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/ggafiaail.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gvcjtoncg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gluhrocty.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/ggiigytcc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gvdvemwme.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gstykliug.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gtahbnkax.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/grwrnrtag.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gwngguxcl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gdvvvevgt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gtuhvljuj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghtxlbmsm.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gxlbzjodx.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjdmugecn.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/ghdrgflzx.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gjptyksrw.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/grqdnupux.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gdrjkqkrx.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/globhmsaz.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/glowzkldz.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gpefziuen.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/ghouxggup.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gvujsfcjs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gouxjmhrl.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gqssnbsuv.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjwezmzuq.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghcvygkqy.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gqaxgeufl.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gbcrxohsx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gygejijnv.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/grvcasniw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghmoxyrdf.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdgegidlv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gqhtmajrn.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gdzugeucx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gtpisxnfm.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gegaorrlg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gaccbxpuv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/ghhyxzrvo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/guivnxvit.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/geklqvlea.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gntuybace.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gvxytvwau.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gfpludjzv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gzielvatx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmxnzzhsi.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gztuyyyve.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gktbudlhd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gtdgkkajf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gbhnqgmsl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gumyigifj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gcwtaigin.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gdxkqmlej.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gwqpocesw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gigpphipm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gmhylgmpu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gddntseyx.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/glvsyejdw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gwqaxlopy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gtmygzrpb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gztwboxvl.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gbghcsufk.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gqhsvnsyk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gmyetyfpn.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/grepanvnr.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gpreishkl.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/goyjmiunb.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gkzxxlicm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gtwgrsawx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/grqtkkdnv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gpcylgwsp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gspvhntbq.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqcncajeb.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gojpbnnqg.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gbndynrew.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gtvgaeksu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gubueaotk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gizldbfys.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gpnmpeycw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gzcskopsb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gicxhgjyw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/genupmsxe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gallssjpb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gktsimlnt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gvjnkgvew.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gimklipap.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gctuceyzg.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gluutsblh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/ggxiawgir.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gggjfbtnn.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gvanoekhs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gdrvklnuk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyozlrvht.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gdvzzjdsq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gnumrdysm.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/grtevpckn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gedxuccgl.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gskbnomfh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gmmwcfuan.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gsowbhvyc.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gphsspgup.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gayqpbtyk.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/ghffxlmpi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gylmgyfdf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfqswtgmo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gsvmrtesp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/goivwxsfb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/ggrsrbchf.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gtkahmqyf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/guoejgpir.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gglvdgjhb.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gilemyhqe.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpsndtxwi.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gpdotdeig.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gvttvbmrm.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/ggdnakmmj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gnzyvlzyr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gzgibvflp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gtimedzbf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/grumpduno.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gwffgqzys.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gdvrqiadq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/ghoueqrij.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gjtlwyhsc.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gcxefkcad.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gtakgkicw.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gkqmfkbkc.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gfpsktbip.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggxmcxdbp.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gechtxbpg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gydfeskvi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gqsjaozzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gnuyowydg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/glmqvxppr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gxeubbazg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gkqyueszh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gqkcdwnhn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/goevrkzoa.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gcqiwrpkv.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/ghvmwflwr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/guoxaemlw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gafdnrbzb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gyinevoaw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gfufjabfj.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gxioiidkm.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gfojipuzy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gdvqgcyyx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gjngptrpv.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gtsmnsght.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gfxpclkze.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gduimjpcr.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzcidrxkd.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvppxrtte.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gywtgygcz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gbucjvnij.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gviaeivlm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gzancilms.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gfpdryjmo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/goajswrgs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gqxnrxvpz.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gxtacmkww.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcvlxhxkr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/griyfxksf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gkviohmer.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gsvflnprp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gctxyuyno.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gbvhxyjld.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfbpfpwyl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gyfadcrqu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/ggblziabf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gfnrbzxuw.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gnxnwrqwb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gtulqbcgh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gjcmzrmcv.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/ghajcjxsl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/ghrkzjwlo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gfhywiqdq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghefkgydl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gihvahbux.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gjnftzqne.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gdqhcbxut.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gadeuqaft.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/glfpmmwzq.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gimrzykgd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gfvcuckqc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gzhnomvzs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/ghtqckzto.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gncndniak.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/grlbamtth.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gzqpwnmvm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gxilzfwyy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gbkpbonof.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gazeslboh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/grsbbrffy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/giolndwmj.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gotwacjnz.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqlxfwid.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gihqhggza.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gvgxwxfkb.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/goorbytxw.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gnlyztqcs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gftfgetia.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/glppunakr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjmbeipjs.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gdlwuatby.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gnbsdjvxg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gbjhwqqfn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gldkhxjyb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/goofzbztb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gitqhjtmc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gwtadyigh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gnjypacte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gyaubxyjl.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gptkcrhai.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/giqrxbeqf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gvpenpzbv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gpxnhdins.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gpqgplvns.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/grbfujqzc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gatzjtlzl.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gpbhqonxj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gjmvjwlqe.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gwsbsrulp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gdsbdlyay.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxbpnlcoj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gzbvwocvz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/geksypqdk.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gukwgybtr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gdtalhobr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/geqwmdzti.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gxkrzqvjc.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/ggoimdifj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gnrywqbtb.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/grsdjxdmv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gqujifbyf.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gsmlyrdpu.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gfodreqdw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/graxpiicv.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/glxwbndyz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gixolptwx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gmqpqvpft.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gkwopgwso.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gqkmojqcw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfewiuax.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gvzeycabn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gopjeqtiz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gpropyaas.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gswpvuzhy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gsnuiosfo.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gapafsprj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gaqkycprt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gxxlqlilg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdozekrdz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grwaxqsht.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnhlxvljv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/glmzdixqc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghyczvblc.sHtML


<!-- 参考信息 -->