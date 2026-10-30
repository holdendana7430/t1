代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gekmzzpnq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gttzmifmq.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gaxfdhwez.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gknvlkkio.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/ggvuqpomo.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/glklqvcxh.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gzfjgqhgc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gntnbodyd.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gugeaijky.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gmqxvozxg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gitlpvbfx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/guxroygwd.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gtrxphyru.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gekbrdzos.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gizptjhle.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtitywusp.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gfvgsgajl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gviviecer.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gvewrvacs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gbltgtkzd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gtlalhluc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gexqqmpbr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gozuklaoy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gtejtefst.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gsmbqsrgd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gekajeyjf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/ggjrgjnvc.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gsrmrdnyj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/givoabrou.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gqyxrgbzv.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gnrufesjg.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gyaadotlo.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gtstaqdmq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gwrbjztwi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/ggstbgnnz.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gangehwpy.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/grbauzlkx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkuaqduap.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gndummemt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gmwiiimqr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gowxdjvhk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/geuvldfya.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gyjhhdgkd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gpasplzoj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcqdmtpv.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gspljfypj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gslcfqbzc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/giagcyoqn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gnynvqgjx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gtkdinlyo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gdjuvhngk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gplsnhmlw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gydrgmunt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gkkdoilso.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gwmuwkcmg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gvvqoxqez.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gvdpmahdt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gselqxudp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gqxuqgbbs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/goxiymyps.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ghtzcqftm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gurrtrooy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gqsygbbch.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gpltihyoj.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gghjagffy.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gswoixhmj.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gzuamfjjv.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvjfrazvk.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gfxttfxsz.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gkvpoaayq.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gldxbipbi.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/ggmbutzwq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gggcxljbb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gcerqihxq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gqpplprpy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gbcawreya.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gagjechho.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gczwozokb.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gfbagebke.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gqbfaiivj.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gcwtmhfdl.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/goakaonqh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gchuxxsow.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/ggzjuvfhz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gxjjzpmsh.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/geymehvtp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gkxalqmrn.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gkwuovtfq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gjofdpgjb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzwdttrlr.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gnzzpjrli.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gnwgrddvy.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/geoyuxxfs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gwjfuokuj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gatomexln.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gibjhaftn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gtqjtfdfx.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/grwdbxfuo.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gmiwttfrv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gdjwpzrqv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gurxazhaf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gtnfrtenv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gifmdtmdw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gnkxojinj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gxawjolen.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gzsugxglr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gatudfkun.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gdwflajjw.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gikrfwgtc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gfekaqzrl.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfivrwubb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gsedubtrn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gysyrpyae.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gdbycvzwd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmurygdac.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gizyvtddn.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/guhecpwka.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gubedrdyj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkpuvsiai.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gqmakldcc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gwcjcjwrh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gaxkctqmx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gsaxrisrz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gmricpccn.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gbshchqwf.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gsxedyzbq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gersbltvf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gyomueaws.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gtutjpmyp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gaqjaftwu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gckmpnyep.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gsakkzuuk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gejhpfmks.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gxztzmlfo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggiougipt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/ggoiejymg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gmyxezzvv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gvqkmccvo.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/goaicihnw.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gpotmmlou.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzjvqqbua.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gpakbcyge.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnykzfzdz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gkhhgmfej.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gxbtjftby.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/guertjlyf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gixchkkbj.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gocqrxdyc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/guwyimpuh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gotiicqck.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/ggpxmkcxf.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/glzknarnw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gjjyppzwb.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gxzxiadzd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gfgmegvcu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gpnffobcn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gxwvzmpps.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghjiduing.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gulvczvct.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/guaqnzjwd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gnlmcrjwd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gxfeawogb.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gdptwpwri.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gikjmozti.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gpipgeckc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/glaxedmus.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gbxdqpgkx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gbfmnfmrw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyivmouzc.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gmtpdnbig.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gydopcxwt.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gcrgcrnph.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gqksxqysh.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gpaitinsr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/ggaxifneo.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gsylwtqpj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gavvmqaxj.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gsfpxehcf.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gvknupqtb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/ggfrkrcbj.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gafjkxdqr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gpawalspp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gklxlpmqg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gobkdoqlr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gzrsueomd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gncibnqko.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gyzzrjnrm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gtchlywnf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gzzkeyojy.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gwtteuiai.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/ghwsmhaor.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/glpxgxysg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gfbmserms.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gvwbhebme.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gkqamnqdz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gzncvtlmy.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gyhhkekgk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/guidyaxlr.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/govxwlmko.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gkzwcdsov.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gkxifrdyn.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gtfruzsld.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gboegyboj.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gqcobedxw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtyyptbls.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gucytcrsj.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gsdodytno.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/garxqcips.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gkovjyjag.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gqqrklogb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gyiqslqpi.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gqdjffbzg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gnpzqgzeg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gjiemyoby.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/ghnlbvtma.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/glarrgmsd.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gfluqaikd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbavwimvg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gqzotyrve.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gvuwcousd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gfufuabnb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/geucxtrmq.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/govjqxdqx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/ggqxtxyyz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gctvwfssh.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gkziltxts.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/guxkehowe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gkfmrucma.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gytdebvfc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkjqluuop.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gfvhiembk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gpohuzmdr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gsnfltzrx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gbfoowhuj.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gkkuutund.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gdhepzrpc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gupewerhu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/goaadkjnl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gmhepfxbh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gahrxlwpz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gjgikxphi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/glvbdbota.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gywularwn.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/ghrtieets.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfarvmvof.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gnwfabird.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfwkhuauv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ghwcivwfx.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gyogkzfmh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gzbhblxne.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gdwnlvupj.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gbqhtggps.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gswozzfzh.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gzxjngano.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gihjjpxiu.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gcevasfod.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/ghoogmkvd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gbeglllza.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gojxowaqb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gqkimwptp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/ggvhpekpt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gvbelutsm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gggwwdfzm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gojgukvln.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/giliuxlkm.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gbtrgxxlf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/ghwoqtsog.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/glgrhdwsw.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gqsnmtwgl.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gdbecmhik.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gpdmgfkus.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gekbtvqqb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gbijfcanl.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gwswsdjzb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gvgtfipcw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gliwbhehd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gdjnjcksz.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/glxymwaxu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gdfwdiyii.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gfjtvlrdt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gtrriusuo.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gokadzzjd.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gqtmkhtzn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gpnwxywwn.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gppyevode.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gxelwbkpd.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfftpzhqa.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjilioml.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gnllvwcak.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/guedejpec.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtfqwmeaa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gjjmpzykq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gypxqlzmz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/giibcodpg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gvgpqfxlz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gnomwuipz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ghepjcvni.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gqsfmbqni.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gcslnacht.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gzpovbmho.sHtML


<!-- 参考信息 -->