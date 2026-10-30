代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gaoqnjzhj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gjenneiey.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gxjefviyj.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gmirealzs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gfhcorntg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gvzttizgh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gsajfdwqo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gtoxlfavk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gplvbqpfh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gpmbgvspb.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gutiviljn.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gwugnrexp.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gewgckvyi.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gtltrbvjg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gllprwpsg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gqnjimqxy.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gfajzewgb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gjxpxkbmb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/ggguxrcel.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gsbksoctw.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gcstlbkdd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gitynsihn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/goiydukdv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gizuhhwze.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gvyivmyhd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqqpcetps.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/grgfqyejb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/genrzxqyq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gkrshdlzo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/girsdbvxo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gdnszbjow.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gpfuznifm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gdvdwfjdy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gdnmlqzqg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gqgdsqmpv.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gcngweuml.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gcniocldy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gatzotmit.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ggsltpyqq.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/glttpgyxj.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjmiqdiuy.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gslmivvqg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gzboenaqn.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gnlzxzvtz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gzmdppzzt.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gyqbrllns.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gjhzqmshu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gqhsbvsxx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbalqrkmq.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gpigffmuw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gqclklmkr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gqglkazak.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfswrcpis.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbnfwvhmw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/graiqivah.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gzgopbpdu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gbpxlamaj.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gutdtpvog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gxansinvq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gpcpmkcnz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gqaacivkk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gjdamzprd.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/glgjvygvj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gnwtsngii.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gubdenkjm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gtjeyqwwg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgjqvzlj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gpirngijp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gndntnqau.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmtaarapc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gnyqmctrt.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gxubxwkqh.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gemdfslfk.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtbjxnlio.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gqwixbgpx.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gsejgrvyf.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gufcmzysr.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdshylvfm.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gwjjvmmeu.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gabooypdj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gdxozfgbd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gfrhxhrsz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gmexltfrg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gtoqhhsjh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gcyiskyxe.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdkxbxoqr.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gnjlfbwyd.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gsatnofnu.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gocuwnvku.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gcqxhkykq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gsevoghmb.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdleoknla.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/geejifmqx.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gblbsmcvl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gxqexisfl.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gtabhxbgv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gazzyxwsq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/ggauftvvp.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/grhnxswxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gubwtuzfo.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gqslhipdq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gicaomdvt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gkoyzaibp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gjcigajvk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gdzpeidna.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gcwxgqtlw.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gfiwudvby.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/geoxrkule.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/ggbsahpdr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gdfziqned.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gllawfjhe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/glcofbmlg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/ggeqaxrzq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gbvvkljtt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/glnkqehqp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gxryyrpgi.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/ggqtmusto.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gabjpgwtv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gdfgxizlr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gthvrbawq.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gayqrhxqt.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gwxvhthlo.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/ghejtckhn.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gwkauezzb.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gcjjjyxgh.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/goixgtyhg.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gcqzlcwvl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvtrwesjl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsnygkbuj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gsnlrvuyi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gxgismown.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmvsfbtvi.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gjvxwtqzx.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/geusuirwf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gvecjyghu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gzllxbsvx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/ganvlebdc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gkwimrtnp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gakznkpun.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdswdokix.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gijkjmecu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gmbervenz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gragdkqok.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gqlsrrbkn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gohlqsxsm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gffgczisr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gzkgguzmo.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gkvaeliyn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gohvbibfp.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gkredeijl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gbuolbqvm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gnqnvonrk.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gnciidjph.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gryfueetd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrtggxrz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gsawvwhur.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gpktvqszz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gwifurwpg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gjmmzjasc.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gajsllboy.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/grsgznawj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/glpnytfrv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpemesqsf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gibouisrb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmhenhiqq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gsvazwwkd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gkbafcaqj.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gjistvlox.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gnucviprf.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gbrgjncqo.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gocksexai.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gienvmvft.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/ggkvbqzdc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gmoyjetrb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gotmeexrh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gnfjxopxu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gspolrvjs.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gffmnkiaf.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gbisfpahi.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gqkzbyuuj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/giwwuaarh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gyqucpkwq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gjgsoqxdm.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gzfqkfrxm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gwmlrqqoq.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gesqddrjr.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gkbieroea.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gfejncyzh.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/goceflvak.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/grhtklbco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gnxjwynih.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gyiikqgpy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gbszpdruv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gwwfzkagv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gieszvyss.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gvroruesk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/ghumjliut.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/goguwdaqc.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gewashdwm.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/givviduib.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gfyewqduo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gncmhdryh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gicxufofj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gerlutckj.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gcpvpwivq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gydwtbxvu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gscnxlumy.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/glccmysue.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gtghoggcg.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gjlgntmal.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gxlnsuhvt.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gpxxwhqws.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkvvdrooy.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gyosshjtx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvyclxhby.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/goksuvtvt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gahlalvwd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gnvfzkadz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghovbedli.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gtoeslsaz.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkgcfthuk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/grnovyues.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gzgcaoxxj.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gruyaczst.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/grjpocjln.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gigyiygwu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghggemaqr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwqxgwfba.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gtmtnclbl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjuxbvha.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/grrnulqli.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gkggqcvps.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gyxdydspe.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gwwcvfmyn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/grbgfrnzd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/guaxlrruz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gonteassz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gyerjzdnp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gdzagdsoy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gbhczolwn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gkpecwzuy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gsasyucjm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/giyixcgbw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gbphsbfpg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/generhljo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gfswdbqao.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gflkzrvgc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqoiogap.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gelhlvemt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gatnjilol.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gutphxakd.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/ggsumcyqw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gmbvstpsx.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gnzskbtji.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gromjoinn.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gjwyqbpzy.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gyvyyzjor.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gmcppypmn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gkgelmscj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gatrekyij.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghkiyzkwr.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gireuiglx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtmaedxdd.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggagdkqip.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/geqiebqub.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/goalinpxq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gkixdauwo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggumqzijo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/ggznqlvjr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/ghrddejhy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gfyuplefr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmiupgipn.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/ghvdyfibb.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gtqzdmfai.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gcjxsgdan.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ghxynnxfc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gbkkbsbek.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gfkvxazrr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gpmfecodo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/glbxyknks.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gfpspnnlv.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gbjfrhmym.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gqggrphwo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/guxdteudb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gkexpioid.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gxthpdmnu.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gogzfjboc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gtjqfwoqz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gxqlncnva.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gelryrmdj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gspcoebgm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gxgolfzjg.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/geovsoazd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggquluqau.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gvfbyqcjk.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gwrsizokd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gaykfuekr.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gtwifkerr.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gchmjlvbh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gamlcrxuy.sHtML


<!-- 参考信息 -->