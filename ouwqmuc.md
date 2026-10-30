代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooxpczna.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gilrgniiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gfayzjmuq.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glqyaiakg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gospmxaex.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvxljrvw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gipgoggec.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftwgybhw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvdrgrio.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gfukgwmiz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gllligjoj.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzznjnij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnftoeyf.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgafrdlz.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnhfzzyw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gncyptcev.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtqsryrx.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaeslmemn.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhwffbpc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gstxjanvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfovphyzq.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gijpjvqvx.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabrcpjsm.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gasxgujvn.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gyuscfeab.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gikgprvfn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gsmpcmhzz.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjkkfcux.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygbzlcrt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gyyldhcsc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gggfaktia.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiskmmkc.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwjxbqbl.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbqksazry.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxnxyjru.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/geaohtiwu.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gjhilcdrx.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gxezbiedp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/ghdbicvxx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevsauchu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gepegmloc.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacijtnqc.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gzluwbyuo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzforjbno.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoontazv.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ghjsvlfat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvqvnqbc.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gsmzrutjt.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghapozchm.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gxzcyztyb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqssthnu.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjqggrvh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gonmycrgr.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgvjwvla.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gorplhuma.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsrpralc.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ghlqpfjpx.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswgmhmuf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtroldhzj.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsyyxgagy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkcgnpkz.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkwrfbia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqfathgb.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gdrfiddpt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gsccupwjf.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwiypvym.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfljuvbbh.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcqokmhj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggfbbaxat.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ggwpyegpu.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/girprmhbf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbbmgkjjy.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gbxugbxei.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigzoamjy.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfqypmpl.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gyrjgacri.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmztewwqo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gimziukxg.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gaobejjmx.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbienjhgk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgtpocsn.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gxqypxryk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhwvjbem.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gswcipcvh.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfzwggthx.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtleqfhfy.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/geyngpehf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqziyllu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxuafzoe.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gmvjncoyx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxjoifha.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghptbnyht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxlsinf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncwchzrv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsriyzodd.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvavrrfhk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gatopxaib.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcljhibg.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/guwptdhld.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gizficxnh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/giukbiioq.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwppetmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glourwrwa.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gkcwmgenm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnddbhapi.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsswzfer.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfmqwqjt.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gphztqrqo.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gtacytcyt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gevuezlly.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejixjsse.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwqstuju.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwckpjkx.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/goydpedyd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gcqsimkye.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzzmrodk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gimpxnpyi.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfquvyqp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gxprptfjs.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxefpzsol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqrotqcm.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/grucngvjd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvwgbcqv.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gltucbnpo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjrugsvn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltunibmy.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gwkwtmfis.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuyhyzne.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ganeboivj.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsdxpoqa.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbdawshp.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhanverl.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/grdycdlpt.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gppyeftkw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtempfops.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gpikerrpb.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/geasmfzpg.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbsetwaa.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gltikvkzq.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsrxqwrw.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkykgcujf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvfoshgl.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjwucdrri.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjtytuur.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvacvxbm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gxwhlthxf.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gxmcgrznx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guafpdwgi.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/goiafckib.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gehwtiuod.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gapralvsd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgnrxiul.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gcepjlppb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/grwslbwld.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwhcrxktz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gdjudizjh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjunxyizz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvnhevyh.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfbcrnghb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrtvcxmb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gldyfrbwd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnbckshpi.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtexekszq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwafixvxv.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/goyrbqqyj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gzjsbwtsg.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/grhsdrirb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gribwyhpj.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gdkynemuq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlczbbsf.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdnuawhn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnucgqqm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgxtabvk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyocyifn.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnyhnxmfs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/glunqrdnx.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gajmxqgpb.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpebfwxd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/glrpywicq.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnqfyfjoy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsbfcjdz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gckzitflj.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/guheqczzz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykgbvrby.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnjpavov.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gchwjkdls.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrrxwxnf.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqunhos.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthdczvlo.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqlmqpijd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkikgjgm.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/golutighr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizeqohuw.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gfcnnvhwc.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gxenzyuuz.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gygpmqwiu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/geuzqhuml.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/goabxxsrt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/ggtcnfofq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoppjswx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geniawwmi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtlqtbfto.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gkflxksbi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdkxpckq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlavshck.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gngubcspx.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gssahwidu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxtgpxqm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gpycncgak.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjlxlzwr.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gwgkxougp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/geoxrwfpt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdwahytm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gutkqpxgx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxcccgdz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gepvdnqhu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gibiaxhoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gigfnjqpe.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdrafsta.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/ghohnckri.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxojrtzko.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvhoxvfo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqalqkyp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntezlyyu.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gihqzginr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gulorkboz.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqjlpwyc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnycyonik.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgkaittf.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxbxwxyqq.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gubjxzmkb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfronahn.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gjjtsecbr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvfjelou.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfccsdybz.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtskjdshg.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdfemjtqa.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtccvfzzj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdhtmoyp.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/giddvjjog.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuxeccqv.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrlvshcv.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxogrdwo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzsedovx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktyxgljr.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpftzmdmy.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjbysboy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdeobcmx.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gahmccpkg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsxqgclu.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gkfohqpxj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgchyati.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gjupqabjz.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gphmbroki.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeqzrupi.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gujnwgzsd.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gywmecmus.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjbukain.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsbtnqjf.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gcgswdcqx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gfxtejjtw.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gtslcuetr.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gssavllnk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapiorlfd.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guhjuozkq.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbilhcqm.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookdrybt.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbfzpoaa.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuhzspfw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gxxzcpqel.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmvvgiuk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gajbganee.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gsisadrxx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxsrsmc.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/givurlcxf.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwainweda.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gelllrjzp.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuvuuott.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjwipbubk.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvswbksq.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gaoclpxbz.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gcsetrxqc.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcksbdjq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ghgcjignz.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gokfuormd.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdwtrzpc.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/ghbkgvysi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqxvtyrl.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujmnxklj.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gvfevkobu.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/grjnfahhv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxasenkqo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwckmaoo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvturzzw.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gsqvarvzu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaowiyfpf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/glzntlxaz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmvdbfcgd.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtssonrfj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/giuvclhks.sHtML


<!-- 参考信息 -->