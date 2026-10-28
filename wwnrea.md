代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtewzfdsxq.html

[R48] awk 取指定列
来源：http://hz.jiagoushi.top/gtiwvsbjdp.html

awk '{print $1, $3}' a.txt
来源：http://hz.feifeiyinyue.top/gtaxruzxcp.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gtbaztgsoa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtbwnrwzdc.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtwilepvjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.vqdsnc.cn/gtwpzqqnkl.html

[R51] 排序去重取前几
来源：http://hz.ydzc1.top/gtewxisaii.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pycfn.com/gtpylspscv.html

[R52] 统计行数
来源：http://hz.zhaomingkeji.xyz/gttdnagtis.html

wc -l a.txt
来源：http://hz.tianlin.xyz/gtgfyvnusg.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtvjursild.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258.top/gtitmqqqbw.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gtzlqesdav.html

diff a.txt b.txt
来源：http://hz.xuanzx.com/gtagzdbjmt.html

[R55] 压缩与解压
来源：http://hz.jqgufenzy.top/gthzwmlina.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cdnleiting.top/gtwegipgmc.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtketbhqlt.html

scp file user@host:/path/
来源：http://hz.jianghu66.top/gtxbsmvonj.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtpszjagss.html

ssh user@host 'uptime'
来源：http://hz.xuanzx.com/gtmvwqddxv.html

[R58] 下载文件
来源：http://hz.hammf.cn/gtmxtsgwpi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gttkxaucsg.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gturupccoz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtjbwztmfr.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtcwjkyeco.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtnhevguxm.html

[R61] 磁盘占用
来源：http://hz.cucudq.cn/gtwihbnyya.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtmqxnqvsp.html

[R62] 找最占空间的文件
来源：http://hz.xuetiantiany.cn/gtredeyuwd.html

du -ah . | sort -rh | head -10
来源：http://hz.tian-w.cn/gtvzbwgvbt.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gtqidbmsxr.html

free -h;  ps aux | grep nginx
来源：http://hz.zhoulong.xyz/gtgjmbtkwn.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtbilamdis.html

kill -9 $(pgrep -f app.py)
来源：http://hz.haohaochexian.top/gtwoycdmvx.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtsyxhuufg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hywenlv.cn/gtxzpvlfjf.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gtarucwnyd.html

crontab -e;  crontab -l
来源：http://hz.zhixingplan.top/gtjhvuwlgo.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtkytmzwbn.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtzpfevqzf.html

[R68] 计算文件校验值
来源：http://hz.ppjwa.cn/gtjvxqsgmy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gteuzroikx.html

[R69] 生成随机密码
来源：http://hz.smart0.xyz/gtvjmvakgh.html

head -c 16 /dev/urandom | base64
来源：http://hz.ehwqpu.com/gtkccpqnny.html

[R70] 时间戳与互转
来源：http://hz.gaohongyu789.top/gtuukcmxuk.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtwrshkhnk.html

[R71] 日期格式化
来源：http://hz.pengpengdd.cyou/gtncdydtto.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yanxiufei.cn/gtxcpsoqhz.html

[R72] 等待端口就绪
来源：http://hz.316326.xyz/gtgyozsgjz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtwrjjteff.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gtcjdrjvpd.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtpktencyn.html

[R74] 批量重命名
来源：http://hz.chenlongwang.top/gttmlelylu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenzaomai.com/gtmxtaqshd.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtromvuvbv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sufxvd.cn/gtvokgsswa.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtgwlyqfvd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtsuwclzer.html

[R77] 读取用户输入
来源：http://hz.nanxinkj.top/gtfppfwwly.html

read -rp "请输入: " ans
来源：http://hz.cqqwz.cn/gtsrvkmnte.html

[R78] 交互式菜单
来源：http://hz.cheryme.top/gtsbqnidex.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtrzqsrjtx.html

[R79] 解析命令行选项
来源：http://hz.xingfuxueyuan.xyz/gtcwhmshmq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtvllwhfap.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtzpnwbcvl.html

time ./run.sh
来源：http://hz.havefunace.top/gtkvnmhteu.html

================================================================================
来源：http://hz.dianchejie.cn/gtibkyyzpp.html

S. C / C++ 专题
来源：http://hz.ydzc1.top/gtklmxgucg.html

================================================================================
来源：http://hz.jinqigfzy.top/gtohteyooi.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gtluqfowun.html

#include <stdio.h>
来源：http://hz.sysykeji.top/gtsnplpczp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhixingplan.top/gtfjrtwfrs.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtzzgluzqw.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxuanxn.top/gtlugcdqvv.html

[S03] C：读入整数
来源：http://hz.ivvv.top/gtrkcufard.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gtmqoakucn.html

[S04] C：字符串复制
来源：http://hz.meibo888.top/gtruhwgmvu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxuanxn.top/gttdgfxvxx.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gtycatwxfi.html

strlen(s)
来源：http://hz.gotoacloud.top/gtugihzgod.html

[S06] C：字符串比较
来源：http://hz.nanxuanxn.top/gtluowiqoq.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gteyyhjxqm.html

[S07] C：数组遍历求和
来源：http://hz.ydzc1.top/gtrjyxoenh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtotbncjpw.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtiwscchqe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhiwuduotai.top/gtlnpvnxhj.html

[S09] C：结构体定义与初始化
来源：http://hz.xylfe.cn/gtrfqhljus.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydzc1.top/gtsdejakbn.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gtmduwfrsk.html

int *p = &a;  *p = 5;
来源：http://hz.xuetiantiany.cn/gtnksjtbcw.html

[S11] C：逐行读文件
来源：http://hz.nwbrower.top/gtduxgqush.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yvedp.cn/gtmsudcsrd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtjxapevvq.html

fclose(f);
来源：http://hz.redwolf501.top/gtozoamgbm.html

[S12] C：写文件
来源：http://hz.wangshuangyany.cn/gtnnjxlqtq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.haohaochexian.top/gtskiaaovm.html

[S13] C：宏定义
来源：http://hz.jinyuanbaomall.cn/gtokmdqcfc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigfzy.top/gtnrtyborr.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gtnbomgwiv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jyoumei.cn/gtneponbhd.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtrfgclldx.html

(double) a / b
来源：http://hz.hammf.cn/gtpfufwwyb.html

[S16] C：位操作置位
来源：http://hz.zhaomingkeji.xyz/gtopndylks.html

x |= (1 << 3);
来源：http://hz.mhx1999.top/gtkmanouxe.html

[S17] C：安全拼接字符串
来源：http://hz.yanxiufei.cn/gtsqkycfyu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtsbebtaqz.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gtrmewmlsn.html

int main(int argc, char **argv)
来源：http://hz.zhaomingkeji.xyz/gtnitzsldn.html

[S19] C：快速排序
来源：http://hz.c1oappe.top/gtrnhnmqbl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtqbeldhfx.html

[S20] C：二分查找
来源：http://hz.ydzc1.top/gteqrogako.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gttxbeucul.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtoerydokq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cheryme.top/gtsuxgwxyi.html

[S22] C：字符串转数字
来源：http://hz.316326.xyz/gtztsryttz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gteapksdgs.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtvcjpoleu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sufxvd.cn/gtxvwnlvvh.html

[S24] C：获取本地时间
来源：http://hz.hywenlv.cn/gtqelntesa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sweek.top/gtdjokvgeg.html

[S25] C：内存拷贝
来源：http://hz.ppjwa.cn/gttimtwbiz.html

memcpy(dst, src, n);
来源：http://hz.sufxvd.cn/gttxdsmcja.html

[S26] C：内存清零
来源：http://hz.jinqigfzy.top/gtsudkduqd.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gtrxiafzft.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtqeexqext.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtcsnfggtw.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtsjdesspi.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtvsdmjoxd.html

[S29] C：变参函数
来源：http://hz.cashguo.top/gthvfsvrad.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aizwys.cn/gtlxmnsyyg.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtbdmkdpkm.html

#ifndef X_H
来源：http://hz.hammf.cn/gthtwzhbkb.html

#define X_H
来源：http://hz.jlsjyb.cn/gtwllelina.html

#endif
来源：http://hz.yvedp.cn/gtagvrcvvj.html

[S31] C++：Hello World
来源：http://hz.jqgufenzy.top/gtxcrtgrro.html

#include <iostream>
来源：http://hz.pengpengdd.cyou/gtvrqgtpjz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinghuilouyu.cn/gtjcbktzta.html

[S32] C++：字符串
来源：http://hz.xylfe.cn/gtsmgindtf.html

std::string s = "hi";  s += "!";
来源：http://hz.zdqjudy.top/gtfkusjfsz.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtqvbrxvrj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.havefunace.top/gtwlfdjbsl.html

[S34] C++：遍历 vector
来源：http://hz.zhiwuduotai.top/gtvtnvaolg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuanzx.com/gtlzzetjmx.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtywkfivkf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtmqkpjgif.html

[S36] C++：unordered_map
来源：http://hz.tianlin.xyz/gtzvgfsrnc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtknxxwson.html

[S37] C++：set
来源：http://hz.jiagoushi.top/gtwdsswtte.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtinxpqiut.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtxngtibpb.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gtljfmafdo.html

[S39] C++：自定义比较器排序
来源：http://hz.ydjk.org.cn/gtytfalkue.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinghuilouyu.cn/gttcichthd.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gtemfgqijm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gtxpsocvkd.html

[S41] C++：类与构造函数
来源：http://hz.xinyue.icu/gtwmdnxsjc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuanzx.com/gtsujgcaaz.html

[S42] C++：继承与虚函数
来源：http://hz.zhixingplan.top/gtjbtvydut.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtzrjcuyks.html

[S43] C++：智能指针
来源：http://hz.zhijiandao.cn/gtsizzlodo.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtsjnptawl.html

[S44] C++：引用传参
来源：http://hz.shzxlz.cn/gtcrgboegy.html

void inc(int &x) { ++x; }
来源：http://hz.sysykeji.top/gtnjayjaju.html

[S45] C++：lambda
来源：http://hz.jqgfzy.top/gtbzxrkizw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangshuangyany.cn/gtgbbzcltn.html

[S46] C++：函数模板
来源：http://hz.zhongyouzk.top/gtefllcjmc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenzaomai.com/gtykydzueh.html

[S47] C++：结构化绑定遍历
来源：http://hz.feifeiyinyue.top/gtnngprhnp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.dianchejie.cn/gtmgiixbop.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtvgyznglh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtmclusoin.html

while (std::getline(in, line)) { }
来源：http://hz.zhixingplan.top/gtpvydqbto.html

[S49] C++：写文件
来源：http://hz.sweek.top/gttfesipve.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cqqwz.cn/gtlldxkfcg.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtzwlifygo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gttddittur.html

[S51] C++：显式类型转换
来源：http://hz.chenjidiqi.icu/gtozpzudyo.html

static_cast<double>(a) / b
来源：http://hz.pycfn.com/gtjmcihvyh.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtntnieuwz.html

int size() const noexcept { return n_; }
来源：http://hz.tianlin.xyz/gtxccqlkbz.html

[S53] C++：移动语义
来源：http://hz.daxiang520.top/gtfeeuvytv.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtqhavvwvy.html

[S54] C++：异常处理
来源：http://hz.redwolf501.top/gtrnjbybes.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtqufgxxoj.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gttcxhwgop.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydzc1.top/gtdanzyllg.html

[S56] C++：optional
来源：http://hz.jianghu66.top/gtxzyrgito.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtxrtokmxt.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtzcpcglnb.html

constexpr int N = 10;
来源：http://hz.nanxuanxn.top/gtftermhxy.html

[S58] C++：命名空间
来源：http://hz.fzhhl.top/gtbbqrzugv.html

namespace ns { int f() { return 1; } }
来源：http://hz.ivvv.top/gtnfboeoua.html

[S59] C++：静态断言
来源：http://hz.hysaishi.cn/gtsfqxcuhx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tian-w.cn/gtqipypqgg.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtmfxeptdp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtysmzldlo.html

================================================================================
来源：http://hz.nanxinkj.top/gtawzgocjc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ehwqpu.com/gtllgqzqea.html

================================================================================
来源：http://hz.hammf.cn/gtmjvtfgww.html

[T01] Kotlin：Hello World
来源：http://hz.yuxming.cn/gtlavwxdyz.html

println("Hello")
来源：http://hz.xziqi.cn/gtwuqooqik.html

[T02] Kotlin：变量
来源：http://hz.iojbl.cn/gtrkvvlxas.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtwzymqhip.html

[T03] Kotlin：字符串模板
来源：http://hz.hongshengwenyu.top/gtfvtmbzrf.html

"值: $b"
来源：http://hz.cheryme.top/gtxlmbeerd.html

[T04] Kotlin：空安全
来源：http://hz.hywenlv.cn/gteadvucln.html

val n: String? = null;  n?.length
来源：http://hz.nanxuanxn.top/gtsnmiwvhz.html

[T05] Kotlin：when 表达式
来源：http://hz.svipenyu.cn/gtwyxhqlqk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ivvv.top/gtzpdbzemr.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtfrzgzsgu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xziqi.cn/gtunoasqij.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtuevypvvx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.0kj1m.cn/gtsojdnuhu.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtctdqvsqw.html

data class User(val name: String, val age: Int)
来源：http://hz.yj202588.top/gtlierchfc.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtnzvbzecz.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gtofyqavgy.html

[T10] Kotlin：默认参数
来源：http://hz.aizwys.cn/gtrkcxdvwb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.kuanghao11.cn/gtgqhikzpm.html

[T11] Kotlin：协程
来源：http://hz.andypj.xyz/gtueqvxmah.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangshuangyany.cn/gtrfusyrwf.html

[T12] Kotlin：解构声明
来源：http://hz.xuetiantiany.cn/gtmhbkaddi.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gtscuqoust.html

[T13] Kotlin：只读 Map
来源：http://hz.zhoulong.xyz/gtzkiifwdj.html

val m = mapOf("a" to 1)
来源：http://hz.chenjidiqi.icu/gtzxmonyam.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtildetdhs.html

for (i in 1..10) println(i)
来源：http://hz.hywenlv.cn/gtbdgeplou.html

[T15] Kotlin：接口
来源：http://hz.hongshengwenyu.top/gtiylbxaud.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtdzrnmdbg.html

[T16] Swift：Hello World
来源：http://hz.havefunace.top/gtrsrllgtc.html

print("Hello")
来源：http://hz.chenzaomai.com/gtabfhefuu.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtphomhcxp.html

var a = 1;  let b = 2
来源：http://hz.pycfn.com/gtnvngcpjo.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gtmzcshxuy.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtgiskysku.html

[T19] Swift：可选绑定
来源：http://hz.sufxvd.cn/gtpjzrooru.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangkeji.top/gtxhqhaozc.html

[T20] Swift：数组操作
来源：http://hz.jinqigufen.top/gtjhgmumqv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtjcakkasb.html

[T21] Swift：遍历
来源：http://hz.chenlongwang.top/gtrjaetvwl.html

for x in a { print(x) }
来源：http://hz.yuanzhike.top/gtmzyprtgj.html

[T22] Swift：字典
来源：http://hz.haohaochexian.top/gtrhwiwtgl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ehwqpu.com/gtwlouvlso.html

[T23] Swift：函数
来源：http://hz.nanxinkj.top/gtgrkzxadn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.0kj1m.cn/gtwxtomkiy.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtrddsbuiy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydzc1.top/gtqgqcffpr.html

[T25] Swift：结构体
来源：http://hz.ivvv.top/gtymlyqnof.html

struct P { var x: Int }
来源：http://hz.smart0.xyz/gtjgcjbuve.html

[T26] Swift：类与重写
来源：http://hz.jiagoushi.top/gtuvgaamtt.html

class A: Base { override func f() {} }
来源：http://hz.iojbl.cn/gtoarswxri.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtygprksgp.html

do { try f() } catch { print(error) }
来源：http://hz.sysykeji.top/gtngynokek.html

[T28] Swift：枚举
来源：http://hz.xingfuxueyuan.xyz/gtzgeocdha.html

enum Color { case red, green }
来源：http://hz.jinyuanbaomall.cn/gtddhbpguh.html

[T29] Swift：guard 提前返回
来源：http://hz.yj202588.top/gthymqhjpe.html

guard let x = opt else { return }
来源：http://hz.pycfn.com/gtzhbfzght.html

[T30] Swift：协议
来源：http://hz.meibo888.top/gtvjwxbgyu.html

protocol Shape { func area() -> Double }
来源：http://hz.aibaodan.cn/gtzuqiiiza.html

[T31] Lua：Hello World
来源：http://hz.aibaodan.cn/gtamirqdmy.html

print("Hello")
来源：http://hz.hammf.cn/gtnrdzgtdy.html

[T32] Lua：局部变量
来源：http://hz.ehwqpu.com/gtixnpgelv.html

local a = 1
来源：http://hz.zhiwuduotai.top/gtvfkxhkrt.html

[T33] Lua：表（数组）
来源：http://hz.quarkkingdee.top/gtysaniobx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydjk.org.cn/gtrhhhcyaz.html

[T34] Lua：遍历表
来源：http://hz.shzxlz.cn/gtbxchhtzy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ppjwa.cn/gtmwiqebkx.html

[T35] Lua：字典表
来源：http://hz.svipenyu.cn/gtaknfdqhe.html

local d = { a = 1 };  d.b = 2
来源：http://hz.iojbl.cn/gtsxahmtxd.html

[T36] Lua：函数
来源：http://hz.yueranfly.top/gtgopvwczr.html

function add(a, b) return a + b end
来源：http://hz.jiagoushi.top/gtjqxpjhft.html

[T37] Lua：字符串拼接
来源：http://hz.yongpay.top/gtosuanfwa.html

"a" .. "b"
来源：http://hz.jianghu66.top/gtwkivhmut.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gtljymmiaw.html

if x > 0 then print("正") end
来源：http://hz.wangshuangyany.cn/gtfiufgdum.html

[T39] Lua：模式匹配
来源：http://hz.guannengcc.top/gtxkgmyvaj.html

string.find(s, "%d+")
来源：http://hz.yuxming.cn/gtjpueoetw.html

[T40] Lua：元表
来源：http://hz.zhijiandao.cn/gttwoozfre.html

setmetatable({}, { __index = base })
来源：http://hz.smart0.xyz/gthhaxbebv.html

[T41] Perl：Hello World
来源：http://hz.jlsjyb.cn/gtnxvvflmf.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtsoosbtdq.html

[T42] Perl：变量类型
来源：http://hz.daxiang520.top/gtfakmvxzn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.svipenyu.cn/gtnmnjlqyb.html

[T43] Perl：字符串插值
来源：http://hz.pengpengdd.cyou/gtktcezeha.html

"值: $a"
来源：http://hz.yuanzhike.top/gtcbananig.html

[T44] Perl：条件
来源：http://hz.cashguo.top/gtpuppwoet.html

if ($a > 0) { print "正"; }
来源：http://hz.yuxming.cn/gtduceoppf.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gtfwiaxcfc.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtuwpvnjav.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gtvncuylxv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.daxiang520.top/gtmihjgtsh.html

[T47] Perl：正则捕获
来源：http://hz.feifeiyinyue.top/gtkzxjblpc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xingfuxueyuan.xyz/gtbvuxbwcv.html

[T48] Perl：正则替换
来源：http://hz.jqgfzy.top/gtgkxtlakf.html

$s =~ s/old/new/g;
来源：http://hz.sufxvd.cn/gtfhytcnvf.html

[T49] Perl：函数
来源：http://hz.svipenyu.cn/gtgdkvoedf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xinyue.icu/gtzyfnlkij.html

[T50] Perl：逐行读文件
来源：http://hz.xziqi.cn/gtreohsjpu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.guannengcc.top/gtjnszjkjg.html


<!-- 参考信息 -->