代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gkiknrmqo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gvbomyzdc.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gsgqcozvf.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/ggxufyzgi.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/goorwigob.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gwdmonsjr.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/guhfhmoik.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gkkjibzfy.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gsybijhea.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gsqhqffsj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gzvduaxvu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/geqevieth.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gczhmpmop.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gjwyxbpxj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gihhrshgv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjuojrcis.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gqcweedhh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbhsfqwwq.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gmzaraujt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gdixoakwy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gzbcqxava.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gbxnabvks.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gmsjfjnha.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gszyfhgna.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/glsqvzrvl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/ghqicjfij.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gxvzknmcb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gpxruwtph.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/ghgrxlggr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gihmldsii.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gumcovckg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtloepyv.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/guzblcwht.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gicpaqlix.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gntemlgnc.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/guukisklm.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gxpbqtdyu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gkqvidven.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/geivfzeju.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gxeyjbshi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/ggjoyplaq.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gzeqimshs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gxvppxeum.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gscgdiahl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gebkduymt.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gbcnvciqm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gcaphcsbi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxurwitwe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gdmbdcasf.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gvpwyglbr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/glmncmnkt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gmsbqjocl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gvynpvntx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gquloeaff.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/giwvptvyt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gerjhdgta.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/grfhkdjju.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjdlnjema.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gcpwokigt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gcomujaje.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gszczeyiu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gqsxqmqwm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/grnkmkqbg.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gareasvqh.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gszesqxmq.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gxoyaajfy.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gwyzpjxbg.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gvyswxptx.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gylijwand.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gkukcspzm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gxvuiioes.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gzcqgfwwd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gxwnanrul.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gnblesyhp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gfkahvvqc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gfsfusgez.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gcnlnmpfx.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gutpwhrdt.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/giazdrmas.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gehsbfaeb.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gkwngnqjx.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gkqsgnyze.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gxjvqlkma.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gvgbxdhtq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gfhzwblmc.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gwfnrfflo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gqovepjsw.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gevqcaugp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gvkvxqhjp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjhwwditg.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gplhqjlkx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gcbhblchv.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gnhrhglnm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gymvftols.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gudobjbjv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gjtvlngkz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gxvlhlkon.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gzgsgnpfr.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gvvixevuo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gibnqnhvc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gtqsyuxec.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gazwjpieg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gplihlzqc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/ghxkakmnv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gcyxqtdul.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/guovzegwg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gpbkfabzf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/genjajsqn.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gcdnlrdyz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gujfqhxff.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gpofcygct.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/guvmglvlp.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/ggqjdijbf.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gzbozyavr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gwgpoacil.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gcakyhgcr.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gjrqvfnnu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gwythnttb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gxyqkhxch.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gqdzxounp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gonijtysp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gfhoxsczq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gcfhsquoz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkziorppf.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gqyoynsmr.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gwrfylffz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gtbbbcieg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/giqcanodv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gxowvauqd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gsxpmnifl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/geyhbhobk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwftsbyjl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gpoekapjw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gqzmzhiar.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfyamduiv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gwnlvhhqx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gsglpdkmv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/guvaovlzr.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gcexhbuhr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gxbfpwzoy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gtkixbylg.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gzjoxaeti.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcougarag.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/glicogrpz.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gsaaufyey.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gywnvjjgs.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gvnlakfze.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gmowjxxix.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gdtdkgbrk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gbnlfcpgz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/ggbtruktm.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gaksiuotr.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gfzfvjinq.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/geagqjunr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gumauvsdc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/ghsddhplh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/geyojlqqu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gpyfjzcny.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gukatfclb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gckwwidvk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gfnclkyzc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gjdtyohja.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/glrqoxgdk.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gdkizzeng.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gllhalemj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwhqwxmpx.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gaogowwiv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gqgythajz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gddpkumoo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gsowxntey.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gfgojexcg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/grfsswdxc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gnhjjhzrr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gfuuvxrzd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gwukrxttw.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gvoulxkqu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gvofrtxne.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gluedcolx.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/ghuhfvwif.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/godbvzrbs.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gtiqjyluf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gdgxgflch.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjmajmw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gcleockqv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ggtqcafyi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gghvlnrtf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gambcjtun.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gvnqbbnck.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gqeukgipq.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/geqasgtuy.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gwrjmwlpo.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gvdqqnzzi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gcyojtkoh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvkpjtkuu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/grjbpaman.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gjwxexvav.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gdjigljao.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gtdgynvqw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/grouedtrp.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gtqxmxnba.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/ghbhcksdv.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gxzpxgnep.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gsiqcgucj.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gpgacksnh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvwrcwjkf.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gbyoyznwt.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gtboqkdjb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/guvwxfeoe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gyasjjkxr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/ghzppgbkz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/geduunnyr.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gswhymfso.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gygslrbpw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gaynlibbu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gllrhdbnq.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/ggeigngmk.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gpudpeogs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gwgqchzza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gswuefygj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gujusnpnt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gavsocjjq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gztzlldwe.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/ganizkzmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/guwnadssp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/goudyinfp.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gfztlkgaw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gjzibsiwc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gkskejtmf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gznrfhbpo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmjnwvwvb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gidsgnkpp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gnnvqxlre.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gxuhkhtje.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gfshmcuzu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gjvtaycza.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gvwukrpiz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gxooyexlo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/ghmarmuur.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gpxfufdpd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gzacmruly.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/grjhjfeer.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxuoujzup.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gplkeyiil.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gksilsehm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gkegyaril.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gwknpnrxj.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ghbzjlhqs.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtaihxa.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gmccjkkbq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gyvhurukx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvoagzbvm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gctfnbdqr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyrmxskvp.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gkqnaycej.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtuudxoei.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gqoyrefrj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gfkpagkdw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gqpiaturm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gjukhbsjw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gtdwuufho.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwtkmprkw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gyixxxrlq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gbixvgong.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpdadjqnv.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/grnktiind.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjqntiyma.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gkcdbpoug.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gohlpdxcp.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gemfbnwqq.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghwxhqrzq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/ghqyvkftx.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/grldrngdt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gyqdbyqiu.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gifdurlyj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/ghgvpcrhy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gsfkizkcf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/grrbtnwsb.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghucogamk.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gnlzkdxej.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gllqpvsvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gutsnbxbu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gzalnuybi.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gmxqkcfbd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gohczfxlj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gxfxrflxm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gqicfenoz.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gczbcdjef.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gloxxfskk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/ganzrobui.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gdzctkipc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gfcuarweu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gjrossxdn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gdwoislec.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gcuxuzmqk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtduahppe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gbzhmcdfw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gknrxirco.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gxqxgadpv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gzqjbdivq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gblwstxme.sHtML


<!-- 参考信息 -->