代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gmjdficeb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gvdzwsxmy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gkkxjbeqg.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gdyutqyuh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gxrmtiaqj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdnsquisf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gbgqpvdrm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gorjbkbon.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gaaaxgrrq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/glicvrqvo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gebbxurnw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/grmhqfbgv.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/guxnqjdgr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gsznmmfyq.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gfundeotk.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/ggoymkrfv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdmlkmxkc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gbeiqqhrl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gygghuwrz.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gkzewzwho.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gbbphumzz.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/ggdtdrdhe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gqxenagrt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gvsbrfscf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gaivtivdh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvjlclufx.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gqsgbattp.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/grkbhgmgh.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/ghzagsvbo.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gzyrdhvtt.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/glmyhdzow.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gxvqhpeze.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gcqlucezv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gozmcvtlw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gkufsvivo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfzihlreq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/geljcayqt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gtadmudki.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/glutuptbz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gscpdeake.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gbhjbtxrf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggryvlocx.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/glvkipwda.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/grebdlyqw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gjlgjuuwg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/guptssprm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gxlsazxol.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gabaomssd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gcfjenjyi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gcgyqpkwp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/ggypyhggu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gdwxjowoi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/geqowbjkn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/ggzjpfmoh.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gaozoqorl.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtmhaxzkc.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gnlnwhuaj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/geolanumx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gabwhxtpb.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gcgsiimum.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gcerbfssp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gdgosrnvm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gmzjobooe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gbujeatsq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gkyosoiep.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gbyedrmux.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gecgshjlz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gqyhfzjtz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gzetgtyvs.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gaqvqipkg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gfjigtlvi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gbxdvzypg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gervxkxpl.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gamjujyrz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gxhehcklj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gnmczwwko.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gmwskmmsw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gtgeovfbt.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/guwmrfjkz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gfntkvyrc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/getgqtjjt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gtwmwxbqs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gojwjahxb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gjrirlsor.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfftelhcl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gxurccdrd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/guhnkxtzr.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gjongukqk.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvcqqswcw.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gomqyoddx.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gujekpyhn.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gbflayvny.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gkxscfvif.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gsbepowma.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gunjbbvwf.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/glccdeiwp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gcrddbhar.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gmlwfrjef.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gnlqqdiiy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gaxghzxfu.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glzyndfaq.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/goqwbqvyp.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gxekkyqur.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gztdrywpw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gwnwxcukn.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/glqiuweos.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gdhibcgvf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/grvymfbhm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvynvni.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gkkocthwv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gajjtwwkm.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlxnbolh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gytdjtael.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/grvemlkpu.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gbigkqdkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gcinwbena.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gqmntuhpv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gbdzwejoo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gupoixgip.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gixatstza.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gyiafnfqe.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gneczpyqd.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/ghwdxrtca.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gehfscoma.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gckgxnoxy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gegnuvzjh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gcgglltsl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gegwtutny.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gimrdjhfa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gzykcfocp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/ghyoojrff.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gnigtjrtc.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gsvwqqhsq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gmpyxkpct.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gmitctalo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gdgdtoful.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gragnjxvu.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gjdofovas.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbeqwnws.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/ghdoklsiv.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gijceluen.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gzdkhczuz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/guhtzznjz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gzplurxct.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gxmcnnjcg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/grbvtyqap.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gjelwviyq.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxajmczjs.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gxntvhemo.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gskclgfjs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/guijjlmzy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gecjvuaot.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghptsqrtl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gqkaiwwdx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzjfcxdix.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcfqmvb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gcbjobeof.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/glicalqmo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gjrpjjpbu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gtlnqprrw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gsozkaooa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gfnagtomc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gzasjgwxp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gafpaiqxc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gujfkixwg.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gvgrapdfl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gbddscgvz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gkdihcmnn.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/ggwmhcpse.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gxuwyytiy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/geerqesse.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/guwwqsevc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gacdnlssj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/geqgzoqxa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/ghcnbiwvj.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gmcyxjwkk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdpmlnonb.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gdlmydpaq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcuvtootc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gmkmjnqzj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvflgvrhj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gxkymozho.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gxtsufgff.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gxrlujzro.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gbzgtfpns.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gvfejkoys.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gdhcowsfd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gflvrtcqg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/govlohvrf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/ggyomdsmf.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gbzuxelxe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gmojkrstq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gemwcrwhb.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gjjsufxbh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gugutqpar.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gtevadgqf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/geywqjodo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjaqucot.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gxckogtnr.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gsygbxfko.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gzwpegpua.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gmjkeyger.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/ggkvsykgg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnoblsfif.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gwtgidvql.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gjxteulhl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gkwgxzwiq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gwcookqcf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gwtbabkmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/ggxdamrnn.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gfptqwefm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gssgkrvmm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gqtmrrymg.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/geerjxjiv.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gorbpqdwo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gnchrzfcn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gjrndcxnq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/ghxhxcngc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/govtelzit.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gfqicwmba.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gludfhvpb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gqhuierzm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gccpdprbj.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gghiluyif.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/glxlmwely.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsujfcrdx.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gmgqszjsp.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gpfnkgjsj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gfgxvalhw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gacnmgthk.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gapulzprq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gysdlscpd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsbzubsod.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/grbeytdbt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghpjabtuj.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gzvcgywhw.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gjpsojeks.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gwflzgtll.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gcqggafsz.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gkftnvbxr.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gkmmlcvhw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gugbqbazv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxdjgdbfp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/grbwwzigv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggquhwzbl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gsxmhhycb.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gbtwhihrn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gkpxgukeg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gcubstnax.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gpxqziupk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/ghvpbjuxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/grgreefbs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gnqtsgzpb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpnbgmgtv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gydkppvtt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gxkxlhima.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gcnjlclsn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gzerrnapu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gkggwczob.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gmokjwojh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gdoxjtxvb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gznmnwogs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gmvwrbdrm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gtydasdcd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gvmhilcwf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzhuffwvi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gptponmsx.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gufbotfct.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gcayqusgk.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gikcmeryc.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gelxgapbn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gfqozbmqa.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gzevkfuwn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gdreuorvt.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ghqbbmtfi.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gjjfixwmj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnrwwhnlv.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gxjmbexgt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmkspmdex.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcticxkhj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/getjdefwl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnmzfsvpw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gmeepxyui.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxcmwbdyk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/guzhajtcr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gbrneexux.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gotabxrjm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggbsxezfx.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gcucdvyau.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/grtpccyia.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gvozncgwv.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gbhddawex.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbadjgefy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gmgmoutns.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gebhyfdps.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghgutztzr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gjtpsfdbc.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghqezscqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gsebygqra.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfbtbizad.sHtML


<!-- 参考信息 -->