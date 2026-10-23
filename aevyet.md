代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zrtjzytu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yqnsvupo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mszqguhg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3moyfvwvr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wbdlcaqb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3skwemtns.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vmwkncey.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ptutrjxv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pydanbtc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ujqtytmy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ubuogepc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fmctlith.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3iyicwtul.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qdknyrvs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pgywzrjb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrwscaam.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cydbhpws.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3karoloyw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3iqdmbqjm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sxndacni.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uvlnoqpk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wjpqvhft.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bdrsdjpv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3izftlwjy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3swaduyvz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3atbzsqua.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jjxscjvm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cmrkkmlm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zjaowhvw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwxkrhhi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lfwamcyl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gdcpobdw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3tmqgnxqm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3psrdzaao.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nqagnrkp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wajrmwyi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3inebrhdt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3aohmgdcm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mznzmgzt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3arctkszp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zagrykxi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zzxzdnko.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pqucgisl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3krtutuge.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cnpeaowj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3blqhzxge.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gmkkmfan.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qrnyqvfy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mgevxaxi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xolxfhbg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxnkysa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lmqvwxbe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jzheximt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3giltzyou.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gnbhddvs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gwvsdxcw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tyshejkj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jwzudfkp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgxtkxcn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rbazyiqu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ccnpuopn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bsqwtamp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ikjelqyn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jarimzvf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vojkoptk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gmobwihm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3triqcblc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xvpozuaz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xaupoelv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rhkncbqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3esskrugy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3kkupuiyc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3brocuwqf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3asurqxsw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gcbpvhrt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dazbhpcp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3nnxhwvcs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rvjzempt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jdpxbcyg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lnjqsodg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cgtfhboe.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3srgsxwam.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3topigfel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmuhftsy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mjzohron.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvfwndpl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xthcccch.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yujrvebz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xytoykfr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xbedyapt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3iwxdzlpn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bwaiavjb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xussncaa.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3azbzdidx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ozasilbl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bnxzrmac.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fncjvbsz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vxmhhnnn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uqythrya.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3crjmcphq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gtsckudl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3oyzhmovz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ifmekqix.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sxvibmpp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gvikgnbn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ngzhfwlt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nhnyefsw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ryvllwii.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nfmouybx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3koqmiqix.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ovbufjce.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yhtqapof.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dydnkaao.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3czkumvan.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ddrdfbvx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hwofubsi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vanedhrd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kwyniqru.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3eaxmsiez.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lqtfolay.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gbpbshsq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vuafhawi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xrihdchz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vgfjlaae.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kwocyhkw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3afghplsz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gihtztcr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zwppvsdb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ncpxmwmh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xlxawqlk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cvayxanp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kkhpcpcp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wpjddtzg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yhhbowri.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rfhmncrs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yrelsrkc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3goonlmty.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nxzjkbdm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xyljlgtg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ciwddnmv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3opnaopjb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iinljfev.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oahosotc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qcilcwjn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rqlldfwu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vahuddim.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3svvgbjdw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zbbrosyu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zhnmjbey.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3trqsukjh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yyvkgprn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3izbvpsig.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yxsxpftq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frjnfddx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jushpmiz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nijjphxj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mtoebvaq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3awoxzdxw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ppmroloz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vquhesdz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3taoazmsb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wmhjsjbq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xtvzudoq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gjvuznqd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3yggfzlys.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qkeyejpn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bbxfsazb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jancaiqe.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tlplvaxz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3evennygw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vcvssapy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lntbopcf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xnbogsdb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fnonstge.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zpklvlep.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nnykggbz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xpzqkpaj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gbsvmget.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qqxqclop.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojwceumo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xzyyruts.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yzrowywm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zqujkraf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3yjpzighe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3udnidwlm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxitwkge.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dkgwkfwh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bnwfnpdh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zvsbnlfn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jutslpsp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ultykkky.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rdrxekuu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pcxasuii.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zstyhzzu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xvcsvfmj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3sgfanfdi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fjhwkjpg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uvvtswgv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ctbbzgux.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xnfszxkb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ojobwskr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yfrgzcug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uvwmnakw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tambdqra.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yasdlwnh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3iejgobny.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qpvcgwaw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ujpaklhs.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hpuuqtqk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3csbvbqlv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cjtorbkf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zczahkkn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ifezjdha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqdxrahy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ovxmuvhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qewcobwz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gwknuvbz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hpgnepku.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jueigiit.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nvgjzfjb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3emaievmm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bsvdbrzo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gglprpgz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vljgxbnm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3aagcnmwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gwbztmeb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tjfftdfz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kipbqwxa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3amghciof.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tyyqzrdh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3spbhylgl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jvcctrpw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wpbpkmtz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wlzbspcm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dieelpoc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ktddfpys.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vtcvxyzm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3eqhefadk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3cjwdgmhp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nmjidbng.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ocumevxr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdxrxbww.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zvbskpcm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ohlflyyp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rnvmwrxg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ftrqhqrq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uauczcxs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ufxcofur.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hmscftuj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3haajxkjo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qjmkhujn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lhvpxbcr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rfovkwhs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ipndiilt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tnhrcrvl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3awvicomq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xzgzndvx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gofsiwzt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qtboalco.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ykpblbvy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3shrgqumo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3igxuygbr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kdwbovyu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zljwfquo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ahpizdac.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lfixdwke.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vstnrpnj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lpmplfvs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qpnasanx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kunxlkwu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zfimehhs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ayxoojbs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xswwlubr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3epsonxsi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wthxzozz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3nzjkbfuk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pmcbtbzn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iaveijaa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3padfqfqs.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xtomzipy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3krgbmmev.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ugcojfud.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gcbsvxty.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3whyvfmmp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3eqhghmyw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ksbumrmc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmnqqyny.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xbhiaqcz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lnwnpnty.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eujozset.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3iryjzbqv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rtqegrax.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aogkehda.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3chemykom.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3eaoaytcf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3trmisebi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hqspouwq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kfxtxdpj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pcoueyqt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kmucbpbt.html


<!-- 参考信息 -->