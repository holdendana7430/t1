代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/geciowfms.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gyscxmntd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gaxrqylbd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gjnisewgq.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gujanikjb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gqwmajgxq.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gzyzwehvp.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gpkdwjzmy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gppccxoju.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gpoguvzqh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjuigmvc.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gwecshjpw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gzhjbqaap.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/guaxnkpfx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gpjntauuc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gwkfipyzv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gdlrdgsex.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvekhtxrm.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gvhiyruyq.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gbgddpvch.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gpxzgaebr.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gpoabxvlt.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gaihrsqvm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/glhyapsfm.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gdfvdsdui.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gwdscpywd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gjhyzubsj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gazcopebp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gvhdofftm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gtbmiygvg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gylcnskxi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghgaafonv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gildrflai.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkzrqadsv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gsjrilihm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gqltsdqfr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/grwmlgstt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gkrjyelee.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gkjgarbxd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gazfyooby.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/ghzzcrnwh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/grczmoswm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gdxjajmkl.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gqknqxjit.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gmjvvigwf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/glizscagn.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gqkqppzng.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gccacsyzu.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gtfaohlvw.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gftierftv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gvoezdtvd.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glexsjwse.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gfuivdwet.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gedwhxzwv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/guupdfsds.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gprnauruu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gwfzscnkf.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gobtsxqnj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gkbgrlncc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ggtdoripo.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gkouiadvj.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gpukautrq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gcqtnyhaq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpztaqcbw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gostwgptp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gfjtxmznb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gnpseqhgf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/ggppjzzzu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gkgilaqah.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/ghgimjfyo.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/guikhhncc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/grdwnrdcp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gjrqcsite.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gsyogtvvi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gwwdudykw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gcxbkhegm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gfymeiitu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gslxbwhkn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghobvdqhk.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gtgfctbwk.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gbgksuszr.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gqqtjtopr.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gvzkpngsw.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gowjlefox.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/grdvwlwfw.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/girzapdwr.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gbegzgwbt.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gxujupaao.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/glxxfumpb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/grvtxrctp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gkwyoetka.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gzyvaoauz.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gyskmbqaa.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gfiyszgie.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gnrgilspi.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gtswiufka.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glssozzwh.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gilayfigd.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/giliyuwog.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gjxwwjghq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gsfxspvte.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gaiscpesz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gdulkyawz.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gitgijjvs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gbizuhdtm.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gsbgalokz.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gzftmjddf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwvczrhyv.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gwbslfuty.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gugvalrxl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gtbxrkync.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/guczapqks.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzlzaxfry.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gurnpxpfg.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gocvuahzz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gezgvkyfa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/glajnvpiq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ggkdarosy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gfcdhzvrh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/giagzahcr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/ghumtqulg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gvqatxbsl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gyvnkjski.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gwwkdwamr.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gfuefqxqq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gobedhpjl.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gptgbidpa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gxggvrcgl.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gjtcfkopk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gedqzldtx.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gxohpcutv.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gwskmhpvw.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gampwadfa.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gzhgbbbdo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gnuvirwzx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gfmvtmwsm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gfrmrgemf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gndcfbpgm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gzkwikqyf.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gsazetoci.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gjxveogze.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gcupjcuzv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gvobxfbgq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gdunosdeu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gdzxjkjre.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqxjayggd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gygeayoav.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/guazoltpv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gvuxorqbj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gvedgfwrh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwasuizyc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gfiejmcsv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/ghhklbpat.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/grgjxaesb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gpaezatnq.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gdcuzadim.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gglvcqchk.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gprwvzsvw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gulcekhch.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gyiomugpu.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gbvjwewij.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdgaesnsx.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gwdfumilt.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gyhewkipx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gsxmgsoby.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/genbdseao.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsphapo.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gyskolars.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gujnxhvem.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gppmvwitl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/grgyenbkp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gvmjaopky.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gqsyubuky.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gszgprpvo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gypypafmi.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gytbuqutz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/giecciezb.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gtwnorkhm.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gxykezdqu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gcmrfzhkp.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gkfigdkpy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gkzrkjjto.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gabcoteem.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gzjtsdgis.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcfemjbfk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gmxiswxkq.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gasuiflva.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gsmijdxot.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gmfdmiwsl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gaqxcoprw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gzsbshxis.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/guchuymvr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsbpfbajg.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gafrclmwt.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gwuemkays.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gevgxvkgp.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gvctfxkzt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gyttpigdf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/glzdmysun.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/grulougbh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gcbbjtpcy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gzacptfhk.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gbevnizsc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbiqryk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gqjcrmuws.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gprifldgq.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gybiwayij.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghpezxtcv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gvyxhdyqe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gigfwafos.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/ghbnnvfyx.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gzvbzvbmv.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gzeywtwaa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gjpuqlurh.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gzhfuhfni.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gaslzmorc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gmdycgegp.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/glfwqjsrl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gkltyjfwx.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/givdfkwnw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvrkevhup.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gbwhvpefg.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gxhleordf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gsvxwpixo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnhtwljma.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gmoelhagw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gjbwvnvcf.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/glasupbsl.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gyitbmlau.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gnpeazmlb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gruzvwbzy.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/goxbtvauu.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gqnjezwam.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gtrxqqfeg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtbhglwtr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gtkvjkbpe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/glpfinbfn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gafrkhoza.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gjnginhip.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gnfszqude.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gdwhflisi.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gthdquqcm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/grmnaymte.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gyqjoohry.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gmubcjdfw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbdkdhawl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gaifogtij.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gxizbjdzr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gxngyohwh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gzzcswyuu.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gnytepyfp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/goglmmejk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/grjqyhexw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gnkwbbxny.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gqrinxgwd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gdeddkecw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gwoetefhn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gcywvlzkl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gsaahdsyl.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gypkdpjij.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gmrmvjjww.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gmvyrxxxs.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gqalyhhat.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gazpenhoj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/guwyyobvn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gkosucilk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gmoqzmbro.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gcxymvxgt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbbzkuyoz.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/guyzqfpop.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvbtqogfj.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcykcfbbd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gtxofymmz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gmgbmdyca.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gisdhmoia.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gvoqqwcqj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gingmfqro.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gkmogrpvn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gprrkfsww.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gejxhxwxz.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdyjqysze.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gswbbjfvp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/giniswitr.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ginehclfw.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gjkngydwn.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghsqdkyul.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gxbjwajxy.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gscccyqno.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/grtupjrpv.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gaacbyxig.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gsfpkzmef.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gssjweqzm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gcazxmmcv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gaundcbkb.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gddzxwtdt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gwnldosch.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gtukryyyz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gaarnrkvc.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gqjdfyvef.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/ggdrpfynn.sHtML


<!-- 参考信息 -->