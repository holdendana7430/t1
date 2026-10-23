代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvdhfamj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nuvkhrgr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tpmbjnqx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qnhxjhty.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3elwbciwo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bvueghsb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pkblbwhd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kxlotkoh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aawnxifa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3iovughhn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hcmkpwtl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hmbnduml.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3isojwksx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3frmsgpnm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wzjihwaw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jyqygsxu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3hrcszqpf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3exlrmvnw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3exbjaoqx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pqunteiy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yvwipgap.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3leoouzmf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ghsunyql.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3btsccqzc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3sufkuxzm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xhxykbmg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ybvdnptx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3spjkvwfu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nlyycslo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3uisluoid.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrtowcby.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3djofkudw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mseaprpp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pyjffexy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tgqqfplc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mdthurip.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3uxvoarwz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3htgjsjoh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3srwmbaoc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dmznbljv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iittlpnn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zurkvayb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ymviovnd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wslvbdos.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zwtyrfie.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bkiakniy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jiwgbjwh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3isgjekem.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zlhclliy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzjdtbgj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qdqvfedt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zxqefctf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zjtmdvrx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jxljcbqi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jdcnxiva.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cxstnvho.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jzgjbeem.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xdugxbpv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qvwxrmlk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ksnrkrqf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hvaewikj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xsiktdye.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3idpxrcnu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pxpnegwh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tdkjconq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vnazugzt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3thtobnjn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ihxhujow.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3iifuziuw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fdggjwfh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pzrjllom.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ucnqirzh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hlkyadmr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wjwrvqec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dqfskomr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cetjrjkc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qmxvhlqc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3geznfrcl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vxjbuxnv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fvsbvyks.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3htlslwyn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3utqixzjh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wxkllnxz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fwenhbew.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gprladix.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ufhxxswm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qaeigrof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kodgqxva.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bkcpknqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnvjbmdo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kdpwamnb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ntuuudxc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgfqmvvw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ejqhettb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yjcxecbc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ssoroqgz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wjmfseln.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kzkhmrmn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ziawgbvs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vwhfnoap.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qbptolib.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fhmehrkl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bcypyfnx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jxtbjwcr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kmrnnrfa.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iwisywmu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3onxdnbrs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vdbxtnhi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uprqhsxi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nbfyyhig.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3idisvqvv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3viejeybk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uyjgzltm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3viaymhgo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rmbtcwet.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3huhdcdbf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cqzirwki.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rypgosii.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qanmiyhy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3itnlxpyj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vwqewqrg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ccpbfasg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3iyvswsjc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fzeaswss.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnwujell.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqyumfkn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3eysmuafd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnksquoo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zzbuosit.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zdkbaflj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zjvgmbut.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kzvorywo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3naolpaya.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3sbopuksj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oolqficg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ybmkttxn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3klepagqc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3murgcpqw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dfdnizfc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hhuufwep.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yowycrlf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mpmohhph.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nonsbutg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zlijdphx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ypptnirv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3umkenfln.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wqecnhdx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ezefjyki.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kkxrfqzw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjrwemjk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3yofssoym.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3svtwppps.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sghfport.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wobrsalq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ycuqtjbv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dhsglizn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wudeader.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3krweltnk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ltyqcznb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cgmdcrco.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zywyebvu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3aqfpfozp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xcwpbxph.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hplmoiaa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3njtxtdit.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ovqtplvg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jwhdvpaj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dvrxttmm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vfzbvbch.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mrropswn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ppbxzdst.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3irzpcprp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bexrfbfx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xkewndrq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3sqbqekel.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xazdoyqi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3cpibiaqw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pxwtedqw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpbbsibk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nxvsrdyq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rttinwru.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bkhumumk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zchnecgi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cfnwcazl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pyatubrw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xacmefnv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fzogizkj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ngqesrex.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jesjjaly.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xejfntju.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwnhwrfj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rjgeajpo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mxisycvr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzijrxof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3posoynoe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kefqvogp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yezioyhc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qkgzwhxw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qphikrmy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kguinfhu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jluenzrm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mtsbqyth.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3slqqsymo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tqikhofx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jzowsatj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nkcdxpip.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vwqrndwx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yphwirsy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oopadukr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zvypllaj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3oinutjlf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wgxdxvah.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rgrlqume.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pisvtehw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3saniqjuf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kawqjwbz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pdzpmaro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmvlemek.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tgbgiisl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reljxpfy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ptyeewgn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lwplemwu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3otoqkhzv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bctlipzt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3faskjzxv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ktxwkbjh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3prerbzhj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rctoeakq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ixzwxonk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tkhsztuj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qsdorvbh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3btjmrswt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3srthmpps.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3atkyhryv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vldtkuwu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3elwrdukl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtainwjx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3btwkdetd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tuivdnix.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cbaqbmso.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nkcjiibu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fvporeqr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dvxfiegq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvnhtqip.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rkpyzuxa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3llabltft.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iwxmbmuy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vunmsepo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3uancupjp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xbdrwyqm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3clfudwub.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qowsyivc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jswnnalf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gtfobxor.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zxyrajyg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dmmuabnj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wcgkxydo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sixumyph.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ekowjoti.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qnvyqzfn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ujizayto.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3nvtpgtcc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nazpjbmi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3negcwxhf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3odoxqczx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3evnplqwz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3durzlszn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ktcnabfz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3otejhcza.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ycaimndw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3bftgqgzf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nzuzsyva.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lmfcoorh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ancuvyfi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tbqwefmb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cbhhlccv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pywegzzx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rkexukgs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tqodpwxf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gogjscux.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3poaevgsk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ohypjnin.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3knbuhtdb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ywvbpfca.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rsksvrxk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ptnftkcc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3otjebixb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gkoonqts.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xsbeoiuy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yhnbxxqe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnfetzuu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3iybwrsbd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lztsestc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3oqluubgv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ochtjsub.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3auxhetqd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tjuyhiif.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ndjdzvkw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ypfcgihr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3awubnfnp.html


<!-- 参考信息 -->