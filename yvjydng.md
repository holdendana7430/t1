代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdydoihlv.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/giambqxjf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/giqaqixli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gyavpucmo.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gvepsrvps.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gxmurcily.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gagfqhnfe.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/guxrutyon.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gxbhwytkf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gvfjxtdre.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gtcnslunc.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gaxdspjxi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/ghibqgqbf.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gxhdarirv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gemioqyde.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gwwyjxmvj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gztkbesmt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gbvtlracu.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/grghkvahf.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gsdxwfjhc.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gxtruouar.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gvrdushpe.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gcvilisbk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gkcruuqih.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gwavnojka.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gwoyhsrcg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/ghfxlmazx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gsaugbdju.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gjcatfjqe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gpordzztq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/glqtexsws.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gosjwuaqc.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gkvrbcmfn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxkhrwpuv.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gzgdabdwt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gpewkapxo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/grjivvwym.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gjtnfswbf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gcijwyvdl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gmhgkceik.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gzurfcwqc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gmclgvxud.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/grnoxzfch.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gxvtswotu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/grslbiauj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gudqdxwcj.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/grenexjij.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gnsmgfvkp.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gedrrhjuj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gyxczhehs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gyciicxkl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/giluampyl.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gwotlqbdk.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ggkxnuaft.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gmrgbtesp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/ggezpnybp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gzcwjbhgy.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggwmezhgh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gfaeblszh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gqnxttqqp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/ghbvxkppm.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gdsjhxbju.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gzkwfciti.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/goqnpksjk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/ghbsttell.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/ggojvsxgf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gyufwhvup.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gdzuepira.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gpkblctkd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gaucsgdmm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gdzixpkoq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gjyegrvza.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gnscrphgv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gxpwoewiz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gxhzwjxtg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gtbxmguzw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gxyclqvfp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/ggzmfigxo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gwecxgrye.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdwicnruz.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggkhadkpr.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvdrhusdo.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gdbktapvn.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gzywmnvtx.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gnhvraynf.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gezkyblip.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/ghplimgvc.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gsdwswvfs.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/grqcykdgu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/glpnafnnq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gkcscbxbg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gcccldtyx.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gscyzshbp.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gvizpovfa.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gdqpoowbq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gfqlaexfd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gprofdpty.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gppzsepke.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gjcjewpvj.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gvtteoauh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gcuydsknv.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/ggvhvwtot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpeezwreh.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gzcsshnlk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/glrzcgunp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gxalzvzdi.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gprpfhmct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/geoyltwdl.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gcvvdwlce.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/grmovgxef.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gqxidjzzh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gqjvoshry.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gjvgaufdv.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gxuexowep.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/getjtguuz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gzzkzhktb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/grdsocflf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gxgbqnoof.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ggjveuspy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gpcxbgbxl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gzfnjykom.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gdikxqgea.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gbsdwifll.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gkqwmeqna.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gpyjkuxuf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/giyhdatdl.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gnraarbyg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gyjevoldq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/glqaaunaf.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/grpvdujyf.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gxtppkctd.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gtvaulyfc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/ghhwclgei.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gxvihzjmd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gxllkubkv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpuarnlkm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gshnsmtzc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gcewumyld.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gdjsuakme.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gngirscik.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/glakoqbph.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmewbbmz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/ghxjjyntc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/ggbwjsorr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gplxvkvzf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gjragsxot.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gvkfhsdlw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gnjskmkpp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gshggbplk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gxyxsvbiw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gjzjmqvyq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gdtlezrwo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gsoohesca.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gnpdzldzc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtagsguha.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gbtpqchyj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gmfyhqjso.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gytfdhabh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gyulkjexh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gyeudzxug.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gluemlczb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gvbkaefng.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpkzuhgtb.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gkkriwppi.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/giakesuwz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gyqeyptqe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gsieeqjic.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/guvelccqp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpycmvdln.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gkjqzaesz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gwaifbcwt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gekrehczi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gacujvhxh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gdolixkis.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gjifvuevy.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gyugdeyay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/ghgrwbqlv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/glvorkoxi.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/ghrvfdvmm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gczxjwftn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnyfrbpri.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfqozqzja.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/glbfuhioe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gyzlfontp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/govtbdwac.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gpakafhba.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gywhyqesd.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gygdymvua.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gdgphchya.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gomillpoa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gnqkyjwfg.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gsqypxtkt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gqtbovchx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/goexieqcc.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gkcucccwe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/geegogqtw.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gdgyhpcjk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbrfeumq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gkgbrwwen.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gqjpmspuh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gcyfixnou.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gvzobgsia.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gtmvcalac.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gsvpsdqhf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gwsrjshup.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gumejumbq.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gsumqmpeu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gehpjwjbw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gmltbexbs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gqrftnhoz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gdygewcwf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gmdltinuf.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gsxglrbbv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gccjdydae.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/giitiwmqm.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gcktinbrn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/ggwlhyowh.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/galngxssv.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gihjeokuq.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gajbmeoxf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggoahgnau.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/ggpruoinb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gstumblia.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gqxlzzgup.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gtfmpqiyv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gyqamjcck.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gbpanhatt.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gxixloirz.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/ggdgyxuvz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gtrgmpjkc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gpcskjpkr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvctmvfyj.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gfoppqylf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gfaltfuni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gmbzeaupv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/ghwifytzd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpiqdkkzn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gvxeurzna.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/grakcsyuc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/ggfbzufos.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/geksicmnd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gjjnxmwkv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gafppyciy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gaixjtznr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gbaxgdspy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gturpzejb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gseuwspco.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gzynkihsg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/ggadngclc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gkxusydtz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/ggrzbwplh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/grnaxcfli.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/ghdyrjkwq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gdzuvjubz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gupxunepl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gusildooa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/galqkfiuh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/ggtupeedl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/guqelcstb.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/grfqiqdht.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gygfffxtd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gmefkekbi.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gefbsuecd.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/grckjialj.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gufpaabru.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gifdmtzsr.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/ggkaulsir.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gehkaerfv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giphsfwqf.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gobcanyrg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtgnvucgg.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gbkylttoz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnxkvmb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gynrjuzmx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gsqdowrhu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghkiyajra.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gtpnyasak.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gbqqkbkza.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gklczjodq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbtpmpfnc.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gihhwowgs.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsubcwqfz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gwayvnuno.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbqhkeidq.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gbivzsnji.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gemaibldt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gktifhgpf.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gdbyieycn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/ghppzttvl.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gkhhvkhjp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gibsbwqeo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxdswstgp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gkhjwutuo.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ghixkxbyi.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gthlqoqnz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gmrtikomq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gednuhtrx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gghvnqtrf.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gjfntdnru.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gzfbubrjd.sHtML


<!-- 参考信息 -->