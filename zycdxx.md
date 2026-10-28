代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ywan-chungtsiang.top/gtkksxhohy.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtwrxmovct.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gtwvpyespu.html

[R55] 压缩与解压
来源：http://hz.andypj.xyz/gtcsygmggu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtoaqmxfly.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtifbpvvde.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gtuyuquown.html

[R57] 远程执行命令
来源：http://hz.daxiang520.top/gttwobbuyu.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtgmecyngf.html

[R58] 下载文件
来源：http://hz.pengpengdd.cyou/gtsdorotsd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxinkj.top/gtnzpxmvtk.html

[R59] 发 POST JSON
来源：http://hz.cheryme.top/gtfqxbkxbi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nwbrower.top/gtnqgarjjc.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydzc1.top/gthzhthhef.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtnqohebqm.html

[R61] 磁盘占用
来源：http://hz.316326.xyz/gtnghxjkig.html

df -h;  du -sh *
来源：http://hz.aizwys.cn/gtqgvbgesm.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gtgitlqthf.html

du -ah . | sort -rh | head -10
来源：http://hz.xinyue.icu/gtqelxtstr.html

[R63] 内存与进程
来源：http://hz.redwolf501.top/gtnpehdbfb.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtdfxlhffz.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtofnnvmvi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.wangshuangyany.cn/gtgzduwtzk.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtksocbkrx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuxming.cn/gtaiuvbnqx.html

[R66] 定时任务
来源：http://hz.shanyushiyangkeji.top/gtuxphozzr.html

crontab -e;  crontab -l
来源：http://hz.hnxiangtu.top/gtmmcicyuo.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtndrbxfxi.html

openssl rand -hex 16
来源：http://hz.zhengqikj.top/gtbqkqdixs.html

[R68] 计算文件校验值
来源：http://hz.yanxiufei.cn/gtzzglwioi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtxkftxyvz.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gtbvsrsyiv.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtnsvbuzbn.html

[R70] 时间戳与互转
来源：http://hz.aizwys.cn/gtehkjdicr.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtatlcarmk.html

[R71] 日期格式化
来源：http://hz.yongpay.top/gtgckxovon.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xziqi.cn/gtzvakvxhs.html

[R72] 等待端口就绪
来源：http://hz.dashuyun.cn/gttwiagwsx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtnjqxmetl.html

[R73] 分割大日志
来源：http://hz.xuanzx.com/gtfoxmzcrk.html

split -l 1000 big.log part_
来源：http://hz.jqgufenzy.top/gtjbanntkq.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtzgnxluiu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dianchejie.cn/gtfemasptv.html

[R75] 导出环境变量
来源：http://hz.daria6918.cn/gtipqrrwrg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ehwqpu.com/gtjdcxxjay.html

[R76] 使用临时文件
来源：http://hz.aibaodan.cn/gtfynqbhye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gthnrjtvhp.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gteaqhdrly.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtfxgzldfl.html

[R78] 交互式菜单
来源：http://hz.guannengcc.top/gthpfefsfb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtsejzikbs.html

[R79] 解析命令行选项
来源：http://hz.andypj.xyz/gtrqwdduto.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tian-w.cn/gtbwefadqx.html

[R80] 查看脚本执行耗时
来源：http://hz.dashuyun.cn/gtsqjahzfv.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gthdfnuvuu.html

================================================================================
来源：http://hz.hfpthk.cn/gtcjqiqher.html

S. C / C++ 专题
来源：http://hz.jinqigfzy.top/gttdvemgpd.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzoimxqlw.html

[S01] C：Hello World
来源：http://hz.nanxinkj.top/gtvyyxdxfu.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtegrtanuk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gttgzmjsss.html

[S02] C：变量与格式化输出
来源：http://hz.yvedp.cn/gttqzhpmin.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtzoirgkuc.html

[S03] C：读入整数
来源：http://hz.yuanzhike.top/gtcmagbqla.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gtonegawpu.html

[S04] C：字符串复制
来源：http://hz.shuidangran.top/gtsiseczpk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shangyingyoupin.top/gtymyxhowz.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtyzowwbrm.html

strlen(s)
来源：http://hz.yueranfly.top/gtznapvisb.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtdbmuldpz.html

strcmp(a, b) == 0
来源：http://hz.meibo888.top/gtvrtkzaak.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangkeji.top/gtmqitdfqg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shuidangran.top/gtxeopucda.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtorcjazrb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenzaomai.com/gthzxnqcfs.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtxgtslcyq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtayviavdz.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gttikujhzs.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtoxmnrnwv.html

[S11] C：逐行读文件
来源：http://hz.zhiwuduotai.top/gtnxrthlka.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhixingplan.top/gtmvtssetd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.haohaochexian.top/gtxyfoltmn.html

fclose(f);
来源：http://hz.jqgfzy.top/gthfccfwfr.html

[S12] C：写文件
来源：http://hz.daxiang520.top/gtasbrnhtj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtnngwtwju.html

[S13] C：宏定义
来源：http://hz.svipenyu.cn/gtzcznpfvc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.smart0.xyz/gtfhgwskqn.html

[S14] C：枚举
来源：http://hz.gzhubu.top/gtqgbhdoli.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gtlesjhwql.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtbnfwlmnx.html

(double) a / b
来源：http://hz.chenjidiqi.icu/gttvcikagd.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gttndugcex.html

x |= (1 << 3);
来源：http://hz.gaohongyu789.top/gtdnxnjdda.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gtkwbfadrh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhixingplan.top/gtaxrmugee.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gttydpyeca.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtvxcmboyy.html

[S19] C：快速排序
来源：http://hz.zhiwuduotai.top/gtyaduydjt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gtjeddkvgf.html

[S20] C：二分查找
来源：http://hz.andypj.xyz/gtbatuwpzo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtekiyslnd.html

[S21] C：字符类别判断
来源：http://hz.ppjwa.cn/gtnrnidbwu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gogol.net.cn/gthyhzgypv.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtfvqgtiks.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuanzhike.top/gtyjhuwgio.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtdilxhcll.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtdrqamfco.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gttxdkqkrv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gtfdezenms.html

[S25] C：内存拷贝
来源：http://hz.hammf.cn/gtzehurbve.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtsgryfwzy.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtcroucudi.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtwfqlikxw.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gtzrhkeiuv.html

const double PI = 3.14159;
来源：http://hz.cucudq.cn/gthobvqcvg.html

[S28] C：静态变量
来源：http://hz.jinqigfzy.top/gtifxvvvwb.html

static int counter = 0;
来源：http://hz.jyoumei.cn/gtakqddlfh.html

[S29] C：变参函数
来源：http://hz.aibaodan.cn/gtvqosalcf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xinyue.icu/gttdzjwicy.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtjozvvdwr.html

#ifndef X_H
来源：http://hz.havefunace.top/gtulpzqrxr.html

#define X_H
来源：http://hz.cucudq.cn/gtllfgycjn.html

#endif
来源：http://hz.sxryk.cn/gtdjivzibn.html

[S31] C++：Hello World
来源：http://hz.fzhhl.top/gtzndktyto.html

#include <iostream>
来源：http://hz.zhengqikj.top/gtbjpkcjxy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtdiarvvpc.html

[S32] C++：字符串
来源：http://hz.chenzaomai.com/gtvpwmnkee.html

std::string s = "hi";  s += "!";
来源：http://hz.tianlin.xyz/gtmeguwvvb.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gthhiridlp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtvikqgmes.html

[S34] C++：遍历 vector
来源：http://hz.ehwqpu.com/gtfghkntor.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.meibo888.top/gtbmhovhby.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtkwaknmvv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gthijqjbqj.html

[S36] C++：unordered_map
来源：http://hz.aibaodan.cn/gtgkofpkms.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtjehzhcuj.html

[S37] C++：set
来源：http://hz.havefunace.top/gtnyoviuqq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtwnjoeclc.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtbpgqvoap.html

std::sort(v.begin(), v.end());
来源：http://hz.hongshengwenyu.top/gthvxifirh.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtscqtbtza.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtlishwnjr.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtfuuybdbe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtizijcvfq.html

[S41] C++：类与构造函数
来源：http://hz.daxiang520.top/gtldptrkqy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ppjwa.cn/gtvcgxdwbo.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtmeyfpohb.html

class B : public Base { public: void f() override {} };
来源：http://hz.meibo888.top/gtdejsgpwq.html

[S43] C++：智能指针
来源：http://hz.cheryme.top/gtvluvlkrp.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtmuqmuwfe.html

[S44] C++：引用传参
来源：http://hz.wangshuangyany.cn/gtfaybzyzc.html

void inc(int &x) { ++x; }
来源：http://hz.zhongyouzk.top/gticfjrgmh.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gthgujibyi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxinkj.top/gtpttzjoqw.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gtykuiwkzs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangdashe.top/gtkbgvkgev.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gteniumjhw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hongshengwenyu.top/gtkyoaifnq.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtdvvrbaom.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.0kj1m.cn/gtzvzkoqth.html

while (std::getline(in, line)) { }
来源：http://hz.pycfn.com/gtsvwqiytt.html

[S49] C++：写文件
来源：http://hz.hongshengwenyu.top/gtgfvmrdxp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cheryme.top/gtmfbihzmt.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtkdslqovu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtvmyifouk.html

[S51] C++：显式类型转换
来源：http://hz.zhiwuduotai.top/gttnacwzuv.html

static_cast<double>(a) / b
来源：http://hz.zhoulong.xyz/gtkjpwzdho.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gtknvbhixp.html

int size() const noexcept { return n_; }
来源：http://hz.yongpay.top/gteuimdfko.html

[S53] C++：移动语义
来源：http://hz.hfpthk.cn/gtnfrouneg.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtmaolngkr.html

[S54] C++：异常处理
来源：http://hz.daria6918.cn/gtksljchgr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jyoumei.cn/gtgmhtafbs.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtecvtqxpt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gtqtbollyh.html

[S56] C++：optional
来源：http://hz.zhaomingkeji.xyz/gtipoqtkgt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtroyvwamp.html

[S57] C++：编译期常量
来源：http://hz.daria6918.cn/gtgxxotbjn.html

constexpr int N = 10;
来源：http://hz.jiagoushi.top/gttkbnxbca.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtpptywfqg.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangshuangyany.cn/gtraoqtapf.html

[S59] C++：静态断言
来源：http://hz.xylfe.cn/gthsrvurar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtwjtwqzga.html

[S60] C++：遍历并删除元素
来源：http://hz.cashguo.top/gtqvzybnul.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gtbvzfabru.html

================================================================================
来源：http://hz.aibaodan.cn/gtwiexwusd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gtlqdyeqgm.html

================================================================================
来源：http://hz.chenzaomai.com/gtcdzflqcr.html

[T01] Kotlin：Hello World
来源：http://hz.ivvv.top/gtypepoovj.html

println("Hello")
来源：http://hz.ivvv.top/gtgtvmvhjg.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtlmyzmdzw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgufenzy.top/gtedzavjfu.html

[T03] Kotlin：字符串模板
来源：http://hz.shuidangran.top/gtdkqkxtpi.html

"值: $b"
来源：http://hz.zhixingplan.top/gtkwaviiqi.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gttpqoszwi.html

val n: String? = null;  n?.length
来源：http://hz.jinqigufen.top/gtrbvpcvyu.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gttphjlbwl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtgaruxees.html

[T06] Kotlin：集合映射
来源：http://hz.wangdashe.top/gtkjgjdrnc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtiduipukm.html

[T07] Kotlin：集合过滤
来源：http://hz.kuanghao11.cn/gtoigwmjsq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.vqdsnc.cn/gtloghjelf.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gtwftvsscs.html

data class User(val name: String, val age: Int)
来源：http://hz.cucudq.cn/gtvpcsqntu.html

[T09] Kotlin：扩展函数
来源：http://hz.guannengcc.top/gthpgopogo.html

fun String.exclaim() = this + "!"
来源：http://hz.wangdashe.top/gtyohbxxju.html

[T10] Kotlin：默认参数
来源：http://hz.52xcode.cn/gtryzbrbqi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yonumen.top/gthgcecrml.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtmflfcxcz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cdnleiting.top/gtnvymjppg.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtocvvafuj.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtkzemygxh.html

[T13] Kotlin：只读 Map
来源：http://hz.jiagoushi.top/gtdivyubzz.html

val m = mapOf("a" to 1)
来源：http://hz.jlsjyb.cn/gtxrgaaany.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtifzfvoua.html

for (i in 1..10) println(i)
来源：http://hz.9152youxi.cn/gtjrbfkzts.html

[T15] Kotlin：接口
来源：http://hz.sxryk.cn/gtofaxmghs.html

interface Shape { fun area(): Double }
来源：http://hz.ywan-chungtsiang.top/gtuktvdcyw.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtfyxymjia.html

print("Hello")
来源：http://hz.hysaishi.cn/gtgxgaezeg.html

[T17] Swift：变量与常量
来源：http://hz.gogol.net.cn/gtuixgjbkf.html

var a = 1;  let b = 2
来源：http://hz.jyoumei.cn/gtmranqomz.html

[T18] Swift：字符串插值
来源：http://hz.wangdashe.top/gthosvsqyg.html

"值: \(b)"
来源：http://hz.yonumen.top/gtsyjklbrj.html

[T19] Swift：可选绑定
来源：http://hz.nanxuanxn.top/gtmqmxcaos.html

if let n = opt { print(n) }
来源：http://hz.sysykeji.top/gtjwojhyec.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangkeji.top/gtftqseqjf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xziqi.cn/gtgbyrscrr.html

[T21] Swift：遍历
来源：http://hz.jlsjyb.cn/gtbeonjjqm.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtqrfsqtkq.html

[T22] Swift：字典
来源：http://hz.pycfn.com/gtfeuyqfsx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guowangkeji.top/gtyxfhugsx.html

[T23] Swift：函数
来源：http://hz.xuetiantiany.cn/gtxlfxqxuu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydzc1.top/gtkrhvdzkw.html

[T24] Swift：闭包
来源：http://hz.xingfuxueyuan.xyz/gtgjobasjm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj202588.top/gttnzjamjh.html

[T25] Swift：结构体
来源：http://hz.chenjidiqi.icu/gtdyrguwtk.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtspoaxsxj.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gttxjsmasg.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtwflmyafg.html

[T27] Swift：错误处理
来源：http://hz.yonumen.top/gtgngfqiph.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtanjzyevk.html

[T28] Swift：枚举
来源：http://hz.andypj.xyz/gtghuczegk.html

enum Color { case red, green }
来源：http://hz.sweek.top/gttjzakkvg.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gtdznkrnzf.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gtthhsdxyl.html

[T30] Swift：协议
来源：http://hz.hnqzz.top/gtvdaoqypn.html

protocol Shape { func area() -> Double }
来源：http://hz.jlsjyb.cn/gtzsuxfapc.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtnqvmjmdj.html

print("Hello")
来源：http://hz.svipenyu.cn/gtfpjhwknm.html

[T32] Lua：局部变量
来源：http://hz.pengpengdd.cyou/gtxcbwpnyt.html

local a = 1
来源：http://hz.haohaochexian.top/gtweqrwwes.html

[T33] Lua：表（数组）
来源：http://hz.hfpthk.cn/gtoutkcwyw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.havefunace.top/gtdgmozpqn.html

[T34] Lua：遍历表
来源：http://hz.xuanzx.com/gtaosedwky.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hnqzz.top/gttvlitgtl.html

[T35] Lua：字典表
来源：http://hz.snrcjt.cn/gtgpyerhws.html

local d = { a = 1 };  d.b = 2
来源：http://hz.haohaochexian.top/gtigwaakrv.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gteihqquhn.html

function add(a, b) return a + b end
来源：http://hz.jianghu66.top/gtiumhzzqg.html

[T37] Lua：字符串拼接
来源：http://hz.zhoulong.xyz/gtcoxfysde.html

"a" .. "b"
来源：http://hz.kuanghao11.cn/gtbioxvfnx.html

[T38] Lua：条件
来源：http://hz.xziqi.cn/gtaqntkzdr.html

if x > 0 then print("正") end
来源：http://hz.gzhubu.top/gtuclhefmn.html

[T39] Lua：模式匹配
来源：http://hz.mhx1999.top/gtijwfcyea.html

string.find(s, "%d+")
来源：http://hz.dashuyun.cn/gtimsopvmd.html

[T40] Lua：元表
来源：http://hz.pycfn.com/gtlclngdzd.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtfadfwght.html

[T41] Perl：Hello World
来源：http://hz.hnxiangtu.top/gtvknmaeoi.html

print "Hello\n";
来源：http://hz.smart0.xyz/gtfvdwogip.html

[T42] Perl：变量类型
来源：http://hz.aibaodan.cn/gtmjxwmlcb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.vqdsnc.cn/gttwdhuqjr.html

[T43] Perl：字符串插值
来源：http://hz.jlsjyb.cn/gtrqfajrro.html

"值: $a"
来源：http://hz.daxiang520.top/gtyphsmdyu.html

[T44] Perl：条件
来源：http://hz.nwbrower.top/gtqorlsivc.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gtaltdvtrb.html

[T45] Perl：数组遍历
来源：http://hz.cucudq.cn/gtmojitamc.html

for my $x (@arr) { print $x; }
来源：http://hz.wangshuangyany.cn/gtrmqkwewk.html

[T46] Perl：哈希操作
来源：http://hz.hongshengwenyu.top/gtyembjpdo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.birdmap.top/gtljcqhokf.html

[T47] Perl：正则捕获
来源：http://hz.sufxvd.cn/gtlpbrumde.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangkeji.top/gttrsvkdga.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtdedbolea.html

$s =~ s/old/new/g;
来源：http://hz.wangdashe.top/gtsdbinsaz.html

[T49] Perl：函数
来源：http://hz.yonumen.top/gtfimkguyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xylfe.cn/gtewrluvix.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtvwpmldxi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gthbxnrbms.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.redwolf501.top/gtjemqpajf.html

[T51] Scala：Hello World
来源：http://hz.zhongyouzk.top/gtgmxccwhx.html

println("Hello")
来源：http://hz.yj202588.top/gtnashxuxd.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gtmrfvkjsa.html

val a = 1;  var b = 2
来源：http://hz.cashguo.top/gtdhjbnhpy.html

[T53] Scala：字符串插值
来源：http://hz.zhixingplan.top/gtovivbrbf.html

s"值: $b"
来源：http://hz.xuetiantiany.cn/gtffhnjxyv.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtidegfewa.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.kuanghao11.cn/gtkmyyagmv.html

[T55] Scala：集合过滤
来源：http://hz.yuxming.cn/gtzefdrzux.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhongyouzk.top/gtorfadbkn.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangtech.top/gtwykrlrsi.html


<!-- 参考信息 -->