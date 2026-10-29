代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gtfhcgnbp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gghwlmjco.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/glunozipa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gjcvlxfwj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdlkbvhwh.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/giegheamt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gtpezymoh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gbhhquprn.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gfsguontd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gejyttnzb.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gunpahcuo.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gwzjllrbd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gvxnfbnoi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gycprpukm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gotbcczcn.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gkgpaobpz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gmqmixfqu.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gzemgxoie.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gsczzwvry.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gtloxofzz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/ghjkovwfi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gcsmjakhf.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gxjgrmfdc.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gygdttpwy.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gyzmvybpt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/grgibkwtg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gwyyzctpi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gvlxfpghv.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gvgvrizqf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gasipimad.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gvixlfvsg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gnrwzaqrq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gqtqhhqre.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gdrrpmccn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gvcaktlpw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guvlkeqvd.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gprvgywyd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggdvzitle.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gosmhkohx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/glprkynnn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gozybsjvd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gkrkjdwqe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gnhctsfts.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gbcnysgxw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gxncgfeby.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gmljjlymq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/ghslloypr.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gpthgkqky.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gedaendeq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/ggvjxndgg.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gueyjachu.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gshbnlkfk.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gocycxvav.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gilrfbmxc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/grhiizxzz.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gibxcpghc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gnxggxsaa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwxamxrzm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gjnuuzrga.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/glzhsfffd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/geialvmdy.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gigycvzqf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gonzhgwni.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gvxhvwpjm.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gdjtelgaq.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gmtznuywj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gnpvycxzf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gzenudbav.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gpchwoafe.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gvfuqfzlr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gehodcucc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gvyarpeft.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gzqvpgled.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gbotpgdvc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gnyrbytqy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/grkgiztph.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggzoaexnl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/glrpcqrrv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gnrfynkzj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/glxaudqcy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gfwyggudg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gcyuesqau.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gcutfyvlj.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/ghidytayu.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gakktxvmt.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gavtahrhz.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gsqgvzyic.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gzxzasich.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gliwchjyy.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/godzeoezu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/ghjeuhtux.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gpsztvbll.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gvhqvxuyd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/grmbuaqpk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gpuovhdwz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gbxveywrl.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gauvpocdj.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gvdeaynuz.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gxpwwpvpe.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/giwrsryyk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/glctoslkg.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gjsnfsmqm.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gwnrbcakh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gwzxygnbd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/grhvzmnez.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gbmtsgmxs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggusgtvha.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gcjwnhgdb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gribeiiqh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gqseoqlru.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gomkahpmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gnpppnuns.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpcdlqzzt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gmvknjyqf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gefwgddbq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gvplmmiqn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/glgeagqzt.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gvaxgltrt.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gpfgdjrct.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gjhgnovvj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gapwplwkp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gvuywvvep.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gjsfaxtse.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gzlnwnfqu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/ggrqkjzrk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gohzapybl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gkurpyrmd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/grayqacry.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gntkvdynx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gxiuzrsry.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gatpheudy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gwibmkwvg.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gktzzmcyt.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gruyetsqn.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gjdjvcssg.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gnpaekpej.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/guvttlexd.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gtomlmsvn.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gxxmcbljq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gieehmpkt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gdlhbulvz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gbdoyvtxo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gbczgwtew.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwtcigqc.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/ghbjbupqd.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gkndrsqhh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gwasrohew.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzbgiauix.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gussjscuy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gvtsnpgzb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvragkprr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gocjgggem.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gnenhkrfb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gvadhdmtf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdcauzheq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gaudfxcaq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/ggerixjsq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gbvddylxb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gtqlsrlkm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gggvbhhxm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gpbhqddnk.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gngdpbbfv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/ggonnsebh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gcklzuggg.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gzkgiqxtp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gdyutkjgc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmlprsusi.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gpxszyxht.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/geoaxnuvy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gmjnhrcti.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gplylpdwl.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gflwzggtc.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjvgvpfkp.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/ghcmliezu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/giztlcrpp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gwtllgaro.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gknxzdngp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gsnlhuyvf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gxlujelnk.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/geifqddhn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gobtdaruo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gdjzuedaf.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/ghrdpydhb.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/graegbusm.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/ghvjiixvd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gmlmlucuw.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcowczzng.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gmljively.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gxcnjozrc.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/ghufhaclj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gaxsfptza.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gmsdcofvx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gjvzsrieb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/ggrnwhlwl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/glqrdstor.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gobnutdtj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/ggtlzrzvf.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gzjnhzomr.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gkjbplvve.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gnfdyygsq.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gapmecsmz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gymawfjhy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gwifqrtfi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/ghxupvwcb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtyhrooep.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gxgpirujm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/grvjuzmcw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/giydoqzjf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/grsszxfrq.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gvflspftg.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/goabegwiz.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gmnfwryaz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/govhlxdwx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gjrvpibgy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gizklimou.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gkaxjwcjb.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gcwmkxpdu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gttqduvfb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gciqsqqrf.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gkdooyxwc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gsbnhhxvn.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gykiwtcsh.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/glculqfbi.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gwwjtbtte.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gqyugkksr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gojlmajiw.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gixwmmggb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gfhjqlnqo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwwcyqnnw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gdhobmgbk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gnrsfqdst.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gshgbbfea.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/glhjvibae.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gwodtdzsz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gjfvzorza.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gvfomxkrz.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gkouqgxlm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmuqkwpts.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmlafglmu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/guhmxlsba.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjbtzokvv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/ggjiwqcuy.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gsfwcvziz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gbwfxkrat.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gyyqctbng.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gpyitwkst.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gdgbfuqkx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkwvwweyk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gaqptidtm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjarijmvz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gitdtvvnc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gvuzdvjgp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/guzzizxgo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gxejunznv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gmpxxkqvd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gvxmxsagl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gimxmszkp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gswclmcrs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gxdwryhfq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gwlprqmiz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gjmltzpms.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gtanzwiou.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gryryxmnk.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gktjrdhmj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/grdcohilm.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gbkfaplmq.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gqwhsqnur.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gombmcemt.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gbcnjfwyc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gaihhoqhv.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gfyllnwxv.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggiuufklc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyvqqhiso.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/ggzjjyvlk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghrushhox.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtuwbqhxk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/glzlohehk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gdecuwmba.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gqflzywxj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gipjtfewp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gysyldiii.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gpwtuoagb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gdazjmbov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggbhrqzzg.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gighdcsha.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/glajbbnjz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gubrfjfkz.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gnirholyi.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gbhttxgfe.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gpurwhyjm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghwthgkcw.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gdqfophyr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gbcltslqo.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gzxdtnpey.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gubocqmav.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghzapgtnu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gandrrcuc.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gczkeiglz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpvviufiz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gerfjnxdx.sHtML


<!-- 参考信息 -->