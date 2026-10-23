代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hvsibbta.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ctmovvhi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kupqmfgq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3htlhqiwn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vdbedzhd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hamrekbn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3riuegfhv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zqwpuvli.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qgpblezy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3uapsvzow.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3nqdgzazz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqpmxkip.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3goubjapg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gssljapu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jqoxlflz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fyogmnoz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gunvyuaq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cpdknpho.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3izdutnyt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gkdpfezk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ohikqxog.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jiiqaprb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3irgxkemr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wstgniwe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fgafjtoe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3itkprbwi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rwdyjhut.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xokioyiz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zhuhhbgp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3azmgclov.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3elzvpcec.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3nshfuqdq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fvvrapzj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwzqnfbn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vzzozrww.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mratwffl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jowlhyir.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3aqbpcjiq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yjfkalrw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sbvawdua.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tjhauxye.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3aznvqeuj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3flfhonqf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cgiqvjmj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tgonngpb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3odrmwmyy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nluxdwxc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dodktupr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tlftmgfr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rxjmohfn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tuaomftb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nkwxzose.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hlyeunxp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qoluihas.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bowzcjst.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3btaanedk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lqhjmfzs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qgnwxmbu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jwrmvoyc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3esqjawqr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hcdhwzty.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3phabgvxe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lcfuygbt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3crnpkoyf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rlcndxeh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sbtttaab.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vfnxixer.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xylwuqjm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yipwxlrv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ywqephvk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uszwruek.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nsinhifv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3akubgzpu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sfepnmxh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bztiwage.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lzcjdyck.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vgkmbrek.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfogrkqy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fnmvvrhq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qhojbyjl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3racrlbql.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mxiyppoi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3rsikkurl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pfgffcmt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3czhtyrxc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3sulnlvqx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3apuohshw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlkqquzf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3guhprhnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoqxkpth.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdqbmvwi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ghfxhlqj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqbgvyxp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xppkdsnb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3igypnzth.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zbdzfevy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3naijqbvs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yesmhekz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3drvpatzl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wrzerhio.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qzhrkaau.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3htwcjfgk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3evozkjnb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zlxjolyk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iugmddof.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nsjcrwsl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rrynpcsr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jjtsmxlr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ifilciex.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yergdonn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wnxtvlsh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wfociewu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tgwltsmq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3phbjpmnz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ncfevlgg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zvriuyuy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zajoixog.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xrrexfjp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ddpnyelc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ukllpdnj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ljlaualz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pwvepnty.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hpgqpcjn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3murgclrw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kflvmnvg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dwymknbn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vvocwwuc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3aokbfyhd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qntuicil.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fvxgwnix.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jqnjytkl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ackitmjk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tzycecre.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hhtgdbgy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3uxfcqapj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kxcgpsze.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fqotmnce.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ymgvjkcv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vlhxqyfu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bwogdqos.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ttkgaujw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hzhczslp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xzydrxkk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ikzwrbbg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kubfohji.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gbvxyfwe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3umrtsbxo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vpwjlpoq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ceuykppu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hvmwwrqd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hfvbkfcl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nbarrgeo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vmzifiuy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3goddchmx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jomdxqqn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qyikathk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3krozjbqg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qandetwc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3atzhmvto.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yzztwhwd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3blkgixdu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rfmxencw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3efncvhzl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vbyrgftz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wcdyenmb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nyshactd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ggskfwqm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fddbpxgt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ozwdhzbo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3viyodicp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fmbznlmq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ggxuoiws.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ougtensu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dvrsrqdv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xdhycflz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3eqkiqqoy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvwmpidf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lfiuvxhc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3karmkaoj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dzdovhrx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ghrfmakh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hcyisuyl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ewfgqvrm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysjxvchs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dqyolbwe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ztcmgiaw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bikwvvvb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wjvhujne.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pwtfavem.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dompsdnp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oylvomsq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mmzmywih.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3empkzkjg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dlzazpry.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kgicjjyy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ipntcomq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rmlxsgrr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3daevggoq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fcjfwhiz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rvvelkeg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjjuhcjm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ffgljikl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zokzhbtb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tnvdnxeu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hzlhjbkf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gwyvtuov.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3izbsipwz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gtpyzdba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3aupxnlaa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dvixyopi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qanvshzy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3twzhuugw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3clypnvkw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3neiujvlp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xwmbbqlg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gjnbmohv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gsqsnulz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywgrywkc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fulpceez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsakljqi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ypvkgykg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wejmswkq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dzltgiwd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ldmrebil.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vqcizufo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rrhqyxtr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vybdapjo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3aglzpuof.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bvexpytg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fhdligyv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lfmahsda.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qlemzizo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dvtojtpt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fmtgcgrh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3niomtapm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jvobkyma.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dyecslme.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xpvvaagv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yhatmbiy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zjkzpxwz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cenuzcsu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xyfkelhp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wcgwsntt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bldrmmop.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ndqjaniq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wzkrmeul.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xuzmkqgi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uuctcttp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tmtyogur.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ekzhtwrx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ypiwvung.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gbcmoybx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lzcvozby.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jrzmerae.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hwyrxegz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hqrnmmvi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zyeopiop.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bfirykfm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cjotfgfe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eevhpdmn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ogrfgohi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ufmdkhci.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3juddsktg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwgffoeo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3oamewriv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3afdwghvl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tqxwdfxk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yeivblcd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zymlnzzq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xrafazej.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wlfyfnpa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lihgfbpl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3iwrczyog.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yklattee.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lozsmbbg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3uwnpzppg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tslayqhr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sgyoucqa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bjnsqvlr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pzgaxpfj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cyucymgu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rjceofha.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3klnqibwc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ylzyfsba.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jvlzvhci.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gaycgbwz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qsjrertk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bsnvxdmf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3stgidmey.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tdgvunda.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3afsvzvoy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3vsdgcswb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kpbvpnbf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hhqdavxn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gaqknnjf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tpjbflda.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jeroxvyv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nwrkgbse.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3foawvkgy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3givtcxdp.html


<!-- 参考信息 -->