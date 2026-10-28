代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtlfasnwcl.html

[R60] 只看 HTTP 状态码
来源：http://hz.mhx1999.top/gttilavjdx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtngvuyxfx.html

[R61] 磁盘占用
来源：http://hz.aizwys.cn/gtnuoapfdj.html

df -h;  du -sh *
来源：http://hz.jqgfzy.top/gttikbmuaa.html

[R62] 找最占空间的文件
来源：http://hz.c1oappe.top/gtwncpvszl.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigufen.top/gtpjxqkwkz.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtynhfykzi.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gttpyvfmuo.html

[R64] 结束进程
来源：http://hz.xuanzx.com/gtivphgmsp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gtndtbnwjx.html

[R65] 查看端口占用
来源：http://hz.yueranfly.top/gtdwxhaamd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtignvqmxu.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtfpkeubck.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtznppbwyf.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258.top/gtwyupqozv.html

openssl rand -hex 16
来源：http://hz.jlsjyb.cn/gtxxyxwtvy.html

[R68] 计算文件校验值
来源：http://hz.yj20258888.top/gtnjqiewad.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydjk.org.cn/gtvzcydrcd.html

[R69] 生成随机密码
来源：http://hz.ywan-chungtsiang.top/gtszztljbq.html

head -c 16 /dev/urandom | base64
来源：http://hz.meibo888.top/gttbeopcow.html

[R70] 时间戳与互转
来源：http://hz.pycfn.com/gtofzrvyvx.html

date +%s;  date -d @1700000000
来源：http://hz.kuanghao11.cn/gtvxuegzcr.html

[R71] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtcquupdyu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtpuwaegrp.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtnlyomcqh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daria6918.cn/gtmipeyayl.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gthzpvpbiy.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtwcowtoek.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtrfwubqkn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nwbrower.top/gthwfycpea.html

[R75] 导出环境变量
来源：http://hz.sxryk.cn/gtktetoevz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtpxlxvzdz.html

[R76] 使用临时文件
来源：http://hz.zhiwuduotai.top/gtjdadcbnj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtohhxjucs.html

[R77] 读取用户输入
来源：http://hz.ivvv.top/gthjpclgfo.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtmlgtefms.html

[R78] 交互式菜单
来源：http://hz.hywenlv.cn/gtoxtgknkt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gtfntgfvwu.html

[R79] 解析命令行选项
来源：http://hz.jqgfzy.top/gtumizxxmz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtmztzehwn.html

[R80] 查看脚本执行耗时
来源：http://hz.xuanzx.com/gtjatogfek.html

time ./run.sh
来源：http://hz.yongpay.top/gthcuclack.html

================================================================================
来源：http://hz.yuanzhike.top/gtkgjpmnvb.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtwfejxgsn.html

================================================================================
来源：http://hz.xuanzx.com/gtvixhebsv.html

[S01] C：Hello World
来源：http://hz.hnqzz.top/gtaawzrqwn.html

#include <stdio.h>
来源：http://hz.wangshuangyany.cn/gthiyeigzv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aibaodan.cn/gtaqhjoquq.html

[S02] C：变量与格式化输出
来源：http://hz.yanxiufei.cn/gturfqisyb.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gteotppsoa.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtzqswlcef.html

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtwhtdlwkf.html

[S04] C：字符串复制
来源：http://hz.jinqigfzy.top/gtkblqzbys.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtxfakhahp.html

[S05] C：字符串长度
来源：http://hz.jinghuilouyu.cn/gtvjpgsmlk.html

strlen(s)
来源：http://hz.xziqi.cn/gtnorehoyg.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtfyarxsyf.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtitzjjciv.html

[S07] C：数组遍历求和
来源：http://hz.ehwqpu.com/gtxwhxmjmz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtbygjjklz.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtwvsakzfy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtqhsphvbq.html

[S09] C：结构体定义与初始化
来源：http://hz.jiagoushi.top/gtzdbjcobe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gtxqmixtil.html

[S10] C：指针与解引用
来源：http://hz.zhoulong.xyz/gtdsbklobg.html

int *p = &a;  *p = 5;
来源：http://hz.hnqzz.top/gtimqbmbqc.html

[S11] C：逐行读文件
来源：http://hz.hysaishi.cn/gtzikngpoa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinghuilouyu.cn/gtrxjzykca.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.snrcjt.cn/gtzfatjqit.html

fclose(f);
来源：http://hz.zdqjudy.top/gtsclozhkj.html

[S12] C：写文件
来源：http://hz.jinyuanbaomall.cn/gtmtdjsmwu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangkeji.top/gtmchealzh.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gtbuimfqqk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gtwdcpsqsa.html

[S14] C：枚举
来源：http://hz.zhiwuduotai.top/gtugglqpix.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258.top/gtjheqkcmm.html

[S15] C：类型转换
来源：http://hz.yangfankeji.com/gtjnqujflq.html

(double) a / b
来源：http://hz.gogol.net.cn/gthmyrhqpk.html

[S16] C：位操作置位
来源：http://hz.shuidangran.top/gtdtjrkxrg.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtrurftmbe.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gtqpkqjbxp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258888.top/gttohuvlju.html

[S18] C：命令行参数
来源：http://hz.sxryk.cn/gthufvszfv.html

int main(int argc, char **argv)
来源：http://hz.yueranfly.top/gtqingzpza.html

[S19] C：快速排序
来源：http://hz.quarkkingdee.top/gtwbrypfzz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtwjnvpskd.html

[S20] C：二分查找
来源：http://hz.shanyushiyangtech.top/gtumgkufuv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gturpvmlsc.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtdtumpnqc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtococsofd.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtmmhhakln.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gogol.net.cn/gtmkvavkmo.html

[S23] C：随机数
来源：http://hz.yuxming.cn/gtjfxdcxut.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhengqikj.top/gttoufsxiy.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtbhkqnorc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gzhubu.top/gtjmlvrosw.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtdrvfjyde.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gtuapjroxx.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtyxiysziw.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtlngzbard.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtafxqskem.html

const double PI = 3.14159;
来源：http://hz.jianghu66.top/gtkhbmopns.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gthjaafesq.html

static int counter = 0;
来源：http://hz.316326.xyz/gtcvlvrwpw.html

[S29] C：变参函数
来源：http://hz.cashguo.top/gtzoclxmuf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gaohongyu789.top/gtlpedflik.html

[S30] C：头文件保护
来源：http://hz.jianghu66.top/gtlmrwnbpo.html

#ifndef X_H
来源：http://hz.dianchejie.cn/gtmwgiaipz.html

#define X_H
来源：http://hz.ehwqpu.com/gtcfdlqctl.html

#endif
来源：http://hz.zhiwuduotai.top/gtoxdszixh.html

[S31] C++：Hello World
来源：http://hz.jinyuanbaomall.cn/gtjvzahbek.html

#include <iostream>
来源：http://hz.vqdsnc.cn/gthfwvmfok.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.redwolf501.top/gtywdqfjsi.html

[S32] C++：字符串
来源：http://hz.wangshuangyany.cn/gtkbxatlqg.html

std::string s = "hi";  s += "!";
来源：http://hz.52xcode.cn/gtfffrgltk.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtzicaoixc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhijiandao.cn/gtyunzjmyi.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gttuwolfyu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nwbrower.top/gtkjqjeavg.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtfrdypuxc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtqccyagdb.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtphnftdpw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.smart0.xyz/gtliqycgik.html

[S37] C++：set
来源：http://hz.wangdashe.top/gtkiobettt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gtdzbmxhmu.html

[S38] C++：排序
来源：http://hz.aibaodan.cn/gtnwlsktas.html

std::sort(v.begin(), v.end());
来源：http://hz.sysykeji.top/gtnbmrhyts.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258888.top/gtdcguxhhj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtrhylecfr.html

[S40] C++：查找元素
来源：http://hz.xuetiantiany.cn/gtnhhevyyj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gthkzlfkab.html

[S41] C++：类与构造函数
来源：http://hz.shuidangran.top/gtbjafwxai.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtcglseyts.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtufhgynok.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenzaomai.com/gtopievoqx.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtayxtikux.html

auto p = std::make_unique<int>(5);
来源：http://hz.aibaodan.cn/gtdekhwbwu.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gtvnfldyfn.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigufen.top/gthzegsizn.html

[S45] C++：lambda
来源：http://hz.yonumen.top/gtjvauwkdt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gogol.net.cn/gtofciqymm.html

[S46] C++：函数模板
来源：http://hz.chenjidiqi.icu/gtwfiufwjw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gthyqliwnr.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gtnjplurwy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtchbfrawr.html

[S48] C++：逐行读文件
来源：http://hz.yanxiufei.cn/gtbjipqmqg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yangfankeji.com/gteabfvruo.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtemtkevah.html

[S49] C++：写文件
来源：http://hz.wangdashe.top/gtbfppouaw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guannengcc.top/gtmajcfcmn.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtlraaqfvj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtjkhaexim.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtpdjwcpbd.html

static_cast<double>(a) / b
来源：http://hz.0kj1m.cn/gtxwpjlozx.html

[S52] C++：const 与 noexcept
来源：http://hz.zycfv.cn/gtrnxugmgw.html

int size() const noexcept { return n_; }
来源：http://hz.redwolf501.top/gtllsduqzr.html

[S53] C++：移动语义
来源：http://hz.quarkkingdee.top/gtajjetxka.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtiauagsyu.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gtpynorvne.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhijiandao.cn/gthbbogsas.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtoclrsdqx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hywenlv.cn/gtrfgoycdh.html

[S56] C++：optional
来源：http://hz.jqgufenzy.top/gtadcwoymc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.kuanghao11.cn/gtjtlmpgcg.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtmdiumxxa.html

constexpr int N = 10;
来源：http://hz.nanxuanxn.top/gtxwlyqbyk.html

[S58] C++：命名空间
来源：http://hz.zhoulong.xyz/gtuhnmmtos.html

namespace ns { int f() { return 1; } }
来源：http://hz.sufxvd.cn/gttkvsluki.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtgjuukjga.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtvtdjkxyr.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigfzy.top/gtovgleilr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtzrskhuqh.html

================================================================================
来源：http://hz.ybcxt.top/gtsbnnpgcf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gtvasuvize.html

================================================================================
来源：http://hz.wangdashe.top/gtdseemwju.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtwprhlupg.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtjibchavu.html

[T02] Kotlin：变量
来源：http://hz.ehwqpu.com/gtdecshvsl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtasbpuqjg.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtivdijuar.html

"值: $b"
来源：http://hz.haohaochexian.top/gtsywjdjuo.html

[T04] Kotlin：空安全
来源：http://hz.feifeiyinyue.top/gtrsnxfryb.html

val n: String? = null;  n?.length
来源：http://hz.jinqigufen.top/gthyzzaprb.html

[T05] Kotlin：when 表达式
来源：http://hz.ybcxt.top/gtkdpyqqhf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gtfiycnuqd.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gtjubjuttw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gtdjnpiqbv.html

[T07] Kotlin：集合过滤
来源：http://hz.svipenyu.cn/gtjvqkrrxb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zdqjudy.top/gtjcvykohx.html

[T08] Kotlin：数据类
来源：http://hz.zhongyouzk.top/gtvutbpzur.html

data class User(val name: String, val age: Int)
来源：http://hz.gogol.net.cn/gtbrqdlqyt.html

[T09] Kotlin：扩展函数
来源：http://hz.fzhhl.top/gtpeqeggvg.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtsyhvzvea.html

[T10] Kotlin：默认参数
来源：http://hz.yueranfly.top/gtzkodbevw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtcpoxglvm.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtnetmrzbp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhijiandao.cn/gtieruwcqz.html

[T12] Kotlin：解构声明
来源：http://hz.hywenlv.cn/gtwqkncozt.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuetiantiany.cn/gtaytvnddg.html

[T13] Kotlin：只读 Map
来源：http://hz.gotoacloud.top/gtsrfedvac.html

val m = mapOf("a" to 1)
来源：http://hz.jyoumei.cn/gtxmutilbp.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gtzbfyqmfm.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangkeji.top/gthswtllxc.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gthtqvnhjv.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtjrpqnwms.html

[T16] Swift：Hello World
来源：http://hz.zycfv.cn/gtdbhmblri.html

print("Hello")
来源：http://hz.hfpthk.cn/gtjvjluixa.html

[T17] Swift：变量与常量
来源：http://hz.c1oappe.top/gtdvlzuzdq.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtzvhjsxem.html

[T18] Swift：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtoylhxtyq.html

"值: \(b)"
来源：http://hz.shangyingyoupin.top/gtzhwbvjxd.html

[T19] Swift：可选绑定
来源：http://hz.316326.xyz/gtxzyexrah.html

if let n = opt { print(n) }
来源：http://hz.cqqwz.cn/gtxpnomtwp.html

[T20] Swift：数组操作
来源：http://hz.feifeiyinyue.top/gtxrnxwsae.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenzaomai.com/gtuytswdmv.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtryqygeia.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtzuvmxdri.html

[T22] Swift：字典
来源：http://hz.aizwys.cn/gticylsbiz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gogol.net.cn/gtjealaxda.html

[T23] Swift：函数
来源：http://hz.shangyingyoupin.top/gtuqaewotm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jlsjyb.cn/gtogarcptm.html

[T24] Swift：闭包
来源：http://hz.cucudq.cn/gtskblihfd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cqqwz.cn/gtrccpsvzg.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gteyirkclm.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gtiskyfdrl.html

[T26] Swift：类与重写
来源：http://hz.tianlin.xyz/gtreesrtrx.html

class A: Base { override func f() {} }
来源：http://hz.ywan-chungtsiang.top/gtblejohwi.html

[T27] Swift：错误处理
来源：http://hz.gogol.net.cn/gtbcmzytqb.html

do { try f() } catch { print(error) }
来源：http://hz.ydjk.org.cn/gtrnwymvet.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtzjgxkgyq.html

enum Color { case red, green }
来源：http://hz.0kj1m.cn/gtaivuefwi.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gtcvrelhmu.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gtaauqxvyt.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtkwxzedwu.html

protocol Shape { func area() -> Double }
来源：http://hz.zycfv.cn/gtjipkqfxj.html

[T31] Lua：Hello World
来源：http://hz.sysykeji.top/gtuftssyzj.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtiwetczit.html

[T32] Lua：局部变量
来源：http://hz.dashuyun.cn/gthyucbyyb.html

local a = 1
来源：http://hz.cashguo.top/gtnggoidbs.html

[T33] Lua：表（数组）
来源：http://hz.jinyuanbaomall.cn/gtpyaeiepf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gtorwhbxcb.html

[T34] Lua：遍历表
来源：http://hz.fzhhl.top/gtgmhcfrnc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zycfv.cn/gtpgrgsnil.html

[T35] Lua：字典表
来源：http://hz.pengpengdd.cyou/gtyulqeryp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhixingplan.top/gtahpdooia.html

[T36] Lua：函数
来源：http://hz.cucudq.cn/gtjlvhcsld.html

function add(a, b) return a + b end
来源：http://hz.zhongyouzk.top/gtlgpkiwdx.html

[T37] Lua：字符串拼接
来源：http://hz.jqgufenzy.top/gtrhwpeefr.html

"a" .. "b"
来源：http://hz.shzxlz.cn/gttyrdrkjr.html

[T38] Lua：条件
来源：http://hz.tanke756.top/gtovnmbmir.html

if x > 0 then print("正") end
来源：http://hz.hnxiangtu.top/gtqxjggecc.html

[T39] Lua：模式匹配
来源：http://hz.guowangkeji.top/gtynhzzdpr.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtteruhknf.html

[T40] Lua：元表
来源：http://hz.yuanzhike.top/gtbvezlyiq.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigufen.top/gtvmruncek.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtsqfntjpe.html

print "Hello\n";
来源：http://hz.yangfankeji.com/gtayovfdan.html

[T42] Perl：变量类型
来源：http://hz.nanxuanxn.top/gtnkzfoytp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hnxiangtu.top/gtgjxucquk.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtbmybftej.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtfnqmppfm.html

[T44] Perl：条件
来源：http://hz.wangshuangyany.cn/gtuzydnszb.html

if ($a > 0) { print "正"; }
来源：http://hz.xingfuxueyuan.xyz/gtpmlrkztw.html

[T45] Perl：数组遍历
来源：http://hz.jinqigufen.top/gtnggqsgya.html

for my $x (@arr) { print $x; }
来源：http://hz.svipenyu.cn/gtwqepwekr.html

[T46] Perl：哈希操作
来源：http://hz.tanke756.top/gtzoklwemm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ivvv.top/gtevhxqnki.html

[T47] Perl：正则捕获
来源：http://hz.fengsongda.top/gthmwsmqrc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hongshengwenyu.top/gtnzseodik.html

[T48] Perl：正则替换
来源：http://hz.chenlongwang.top/gtlswwpemi.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangtech.top/gteucijtds.html

[T49] Perl：函数
来源：http://hz.hfpthk.cn/gteqcbllze.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.kuanghao11.cn/gtstrwqmcq.html

[T50] Perl：逐行读文件
来源：http://hz.quarkkingdee.top/gttakhcvya.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtaeufivgs.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xinyue.icu/gtzfsgjmoe.html

[T51] Scala：Hello World
来源：http://hz.hysaishi.cn/gtecjujipo.html

println("Hello")
来源：http://hz.zycfv.cn/gtjblcmbuf.html

[T52] Scala：变量
来源：http://hz.nanxuanxn.top/gtmouxsqfm.html

val a = 1;  var b = 2
来源：http://hz.hysaishi.cn/gtgqzwwomy.html

[T53] Scala：字符串插值
来源：http://hz.yj20258888.top/gteilelywa.html

s"值: $b"
来源：http://hz.snrcjt.cn/gtnhsvodqh.html

[T54] Scala：集合映射
来源：http://hz.yj20258888.top/gtnassjgar.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.bjfxy.top/gtnlqrdwaq.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtfvgaosyq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shuidangran.top/gtrioohvda.html

[T56] Scala：样例类
来源：http://hz.zhongyouzk.top/gtzzqftcgt.html

case class User(name: String, age: Int)
来源：http://hz.daria6918.cn/gtlorzlchu.html

[T57] Scala：模式匹配
来源：http://hz.yueranfly.top/gtkgxmryyr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuanzx.com/gtoedrrfvg.html

[T58] Scala：函数定义
来源：http://hz.cdnleiting.top/gtpiouurzp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jiagoushi.top/gtbqkrljmg.html

[T59] Scala：循环
来源：http://hz.yueranfly.top/gtpcjczkwd.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtxutqzlem.html

[T60] Scala：折叠
来源：http://hz.ybcxt.top/gtwxruqryl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangtech.top/gtnhzgtrcf.html

================================================================================
来源：http://hz.jiagoushi.top/gtommklles.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gtejaacmqj.html

================================================================================
来源：http://hz.yonumen.top/gtcwawvuzg.html


<!-- 参考信息 -->