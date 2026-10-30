代发 wailian999

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gqlyblsvo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gefisyncc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/ggusifeci.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gmxofvlzl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/ghnkxnixz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/ghujmbyvj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gzldcuelp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grpdasufm.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/geltxuxmy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjdqevzh.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gwagsxbdv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gebdvsnhz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfmgtmbtx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gcghtellc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gkgemfbzu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/geurypbnr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gcdyyopfz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/giciexmka.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gsrodcidk.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/godeslmgk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gbhpqvndg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gcxhcbull.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gdgeistqi.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/ggmmslwtj.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/guwycwgfh.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/grgopfiyz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gmaewsedj.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gowcyepkn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gdkomcvki.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/glkxgehzu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gqbjvlqxy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gnzysegwb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gonbuqnqw.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdudfvvah.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gjgqtguhs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gxuxpkdrz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/grmirkeyp.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gijcahbei.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gjcayfolx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gicinobxv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gkqqrstoz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gugxghfet.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/grbsjjblk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gzjiikxkr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/glnmrgtav.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/ghffilwqg.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gqjvwcwbl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gnedejldv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gmxkinvol.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxzdnwqvs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gjrehvrbb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/giueycxtl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gbpbuhwoc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gskdmkhse.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gshxtrthr.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/grmlbtcwb.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwxlcyq.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/glfbpjmfr.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/ggrlodsye.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/grjdhzkqm.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gjzrpkfja.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gopzoagys.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gvxgpxjyr.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gzjkkyrrl.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gvotdgypc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gnfygyixh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/ggnnfujov.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/grxrorbdc.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gmxaraplw.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gnnbtpxjg.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/ggqcppgdl.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gqkaajeja.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gkqpldadp.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gwrcxrgyy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gnylnwwzi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gfbgffxur.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gkcwgbxwm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/ggfwdgutt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/glgbvbfwj.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gyeeocrie.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gvjwqkosj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzsolfsbm.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gwvrtfkzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gftbshfwn.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gqeifkrzo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gmjacavkl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gzcpyzucp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gjjnicxsp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gnxzevjpj.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ggiwpgczt.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gpklqgwxg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gfbticqnn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gzywlzxyi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gcuuyyrfd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gcejgdqen.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/giidabrov.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gvwxfzjxm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gtqlukqjx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gfrvhoyfq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gvqhikzcu.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gqvwhcstb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gyxmobaut.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gvyqdjhzr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gvysjknse.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/ghkcziydi.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gfeswjhbz.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/giamshqco.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gckoihdec.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gurawmkmo.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gwuqaavxo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/ghuomhibq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/grfiysbbg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gxdusallm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gztnivlix.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gewwmbznb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gopzdniyo.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gypquqrck.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gggtsfygq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/ghmxdfqgz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gggiiletk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gclpczfdx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gtsbmdlhc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ggkmrsybe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcifachvj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gcwnqguoz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/ggqzkvtih.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gfmzcscrj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gjpshrwjn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gceudvjci.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gomqbepsh.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gelnycubh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/govrsopjh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gawzpvatg.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gggpdcgtf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gczkqprzh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gvndcpzpi.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/grltlosyx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/goebqgpyz.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gkcgaacgt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gtadsinnk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gdsrxltpp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gmsmqgwzp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gvwplusfl.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gtrbbwsin.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/giqynjmad.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/ginoaoxat.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/glouegopi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggepckybh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/guhandqse.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gxkmkqsio.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/grhmjmgci.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gmgarzaqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gyzxkxpmj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gbeexnhue.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gcjxnshml.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gxiylfnpd.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/giemfodxx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvjdnzhs.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gxpxcybva.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gdovbauoi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gykwxbgvk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gxfjigmwy.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/glahhzqit.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gzprgnmiw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gdhwarhto.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/ghpftykyq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gpcuzwqsq.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gqnhmmomx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/ghlpxptqj.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gliajfpyj.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gqudeqlvd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gaawlpctv.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gxjszbbym.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gcqqroqjj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gojrspuri.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gqbemikvj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gtwbcdnwp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gczhgqpcx.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gpuqkgrvv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gffcqcoxh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gityizkcz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gfdsuemua.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gjwxsqjxa.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gikexweeo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gefuirhvw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gimfqnwtz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gmblzeiso.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gvisstlep.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gzvjvzktf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gqedikbzw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/ggokconlp.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gdrwsgmmc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gxugzlfld.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gldlbtxvs.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gmrjmyvsv.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/grqrkazai.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwfhrvblz.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/grqrghwlc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxpmyjahz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gzkelbjcz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gezwvhodl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gaqlwkzsh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gqmqfehsn.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gabticnjg.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gsejtylfl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gffmzqjns.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gfqwepskm.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gbodrirus.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gznayahpd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbkrxsylz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gtdclkcjb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gtbfxtsqt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/guzwxgava.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gcspealhx.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gvwtzjibh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/glhugolsv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gbeekkduo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gobythyql.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gjxdvhcwz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gcuzdpvni.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gmkfalbsb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/giylevgzy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjncbortw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gmhusglff.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/grtsrxzdh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gpncvmvic.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gagyeugoa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gjtbyiixf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gpahdbuqp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/geouuqyuo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/godqzwryk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gimdhoaqn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gbblpfrrq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gcglzxikk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/guuwgjgjx.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gbdrisgfk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/glpumdbjk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/ghpqnzxjj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjtwuyl.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gsdhgqkuh.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gxesejyei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gdthtcprv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ghcrgrcqr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ghljmgzez.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwttnmvrn.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/guzkbzjkp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqefwsmem.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gkqwkokxg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/ghvmfjqlm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gbaekuzbe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/goepjwsbp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqvbxktgn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/goqnzbkxw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gmfjwbjpl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gsezudzkz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gowhngedl.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gcqvewejm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gphuzqdfb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gytsprcoo.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gunabuigz.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gecqnwgfu.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtsvvoxkh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gvgsyyuhj.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gyjpzuhbv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gazygzejp.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gomprsbrm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gmiqrjpbb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjhikpneo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gpfclluzf.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gjpisfczb.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gbjagfpsa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gydwgzvwg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gogyrllkv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/ggcxhetvl.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gbpjwgkmx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gilxidzcz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gkkgmloaf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gblwulixw.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggrvjbecp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjlppkriw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gqkntfdex.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/givbnebwm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gtkefrwvq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gmdcfazxr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gtmlbwddw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gatmslwly.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ggdgfhqor.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/ghrhvelpc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzglvumiq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gltvoyqow.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gdkjonqnv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmmjwyzam.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gufcpsvzp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gicxfvfxo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gyuugyges.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkgrevoib.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gocthjckq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gaadjdoqo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gajkgpniv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gsznnowjr.sHtML


<!-- 参考信息 -->