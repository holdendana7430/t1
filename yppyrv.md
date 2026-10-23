代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hfbxnjaj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cyhrnvoi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hfedcpod.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xcjiduod.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zqyyhxpx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3szbfsohr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ruclwbvh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bxbhazal.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3arpaqfww.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dejqvxwh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wpfcoaoh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rxnymgkt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3drhgapee.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vefzknkw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mngxwhdb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wnplhfbx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dyshikyg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3raiahdjo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vfbzzlbd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yiuzntfs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nxuicbza.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qxqpzxhc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gohejdkt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kxuhsuyy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gjygxnnn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ghrrvzrr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ipsiztwa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ptoczlpv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3szyyzvlc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fultspiw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bevypptf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tlvdimwk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xhshhlbc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nncsypjl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxegrkcj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nvmuzcge.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3andtygrb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gagiiprk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3haohmboa.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zsiprdsd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vbrmwcht.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dxjftzsz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fyvnkzyk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3lfzqjxeu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3huoflzbf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fdezfren.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ykffbbeb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qvzlytlq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ehpzdbut.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3cehhckfy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3umseuhge.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gjrkhjis.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zxyxueta.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3evfnlueo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3llagsynr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hnlzjtag.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3czpdcsng.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3scodzgwk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ztekpwch.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nfrlvhkm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fnwgeuwf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wtroqrbt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gausstjn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3oqfmqfzm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bfgerspb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3snvlfmbx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3uthtvguf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3issavltj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lwiejqft.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ivisqmto.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vkfptqrb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bfmqsrhp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3atuzgpcu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3afmxfbmv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ithkqfow.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kmhfswos.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3cqyxyjpb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qtdnutuq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lyahurii.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gkqkaseq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xjhuebmc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hkwnhotx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jqznpxcs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ggaotxys.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ctirmwwr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jedhjoqe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vysjkgyo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3satszimw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bgpsyxhh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3icjlexvc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lhqbxnqt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pfgqgfad.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tzcpjryz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ndhpdlto.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3udnfrdcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzqxxddt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gqyrfmqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nakfojnz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mufsqsgh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ujxmccvp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlwivwmf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fgeubifd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ynhrtwbz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xidqfyfr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rofqexpt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bcrxxyyq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vhzgkoya.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zhdwyvqx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjjrhkx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tzkompqs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pzgnvbiu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3abzcjfjw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lhlyebea.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3atapecon.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wqzfrskw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yglmiwfo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cpzinqbj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dddtpnrs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sscqbprw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bcfqzlbg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ohtalrya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3dyfrpjll.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tcwqgelr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghnlywrt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zybqrwjj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kfvumqpe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yaivtuqw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3obuwbrjo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xenhkfnz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xonbosms.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3czdhjoel.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uqeqacpa.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eacfdjbi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eyuoqswy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ilwdwekq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vgtfijow.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fjuiwqbx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3evducgyr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pfhqtjhf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wslwafvt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ymmzwprl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gbrlyyrf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mklkgtzp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3okkgoaid.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ebuunrxb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3aixbnpnx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zmcllvjq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ugwkvqhx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jbeymhrw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3utxtsojs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rpjmcwlu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ljckggnw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hfynjcvs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yiydnpqv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jnatumck.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hafwxbru.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gwafajnn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pngwfmcm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3prqjbjgb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iklumpdq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fuqpjioo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ugcitnme.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zkybqiut.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yjgwobhw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3sasitqgu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrljgxfl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgbxlryc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fmftyxhi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hqohsezd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hwksqqwa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3maqdojpw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbanwpl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ywodisef.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bxhbtsvg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3glzdhibk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vfhtxgdt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xslvtart.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jkasnctr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3apxioesq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qnfdnmpi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3iksqzqzf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3emhsttxi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kcsomlfr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kjnjfunt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ngzwdpbg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wtgpwbnk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmgdygof.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ydrtsxju.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lqomzlod.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xwsqsabk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xyqzgyca.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjqlpnck.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3azewzcgm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zwflvkyq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lttlqjid.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3veavagwy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ggsnpsnw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiattucc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ggfsnxxz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rbxqkylq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bpthaluf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjliwrcr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jccpoaqp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iqjyoymr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zosrggvu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3guvmubrd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nxsgfvlh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mtifbedm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbdgwgok.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ruvrccld.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vbtbbgvg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3iobjltgk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bspzdvrb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rcdwujoz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dzlrptmm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vidhhehp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gueiddps.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xvkpwpho.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ypkhkjjh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gbnqykyq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bxzrtryq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hypgclam.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gbqwhwwk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qoxuruvh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fummhrvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afnqycyl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gbaonxtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szdlwmax.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3alvhbxly.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jwqmivky.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwsyapax.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fbkhknty.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yzeqlysr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aixjhwrl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cybtmkco.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3heysvdph.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cozptwan.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ccwzwmxv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sncmubkf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xuorwsad.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ajjmxijf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ecpmivqk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jalmlzys.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3heypkxfx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3svoraqvl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wzncofwr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rjiduhhf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3iveqemzh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dxauhaio.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dzqmpsij.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pydpnvuq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmylxrt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cwhlftsm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ivemmcsa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cjgqsjew.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xwviyzya.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fjbiyusv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uxcnwwuh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3glxojsjp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkifddcg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gisgcasr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3epcqfcab.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3otqjqzpn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pdvovpqq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vivzfkxi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ckeohwbo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3igspwiuy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3merjxbgr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pphmtqus.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wxnuwhpm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xvtibiok.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zvkfcore.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3phwbffjj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3eoustlzy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bgmltxym.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ajnqtmvj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3snnweawy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mzsyabts.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jmcrikvg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gjoojbtp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ptrgoktv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ptypncia.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bnahnbcj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gnafnbzl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3imsrlgyy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmrbier.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nchseqbu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3idljvqam.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qajvfllr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bpwwbbgl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dvuahpzd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3joxszmaz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3skidppen.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fojudfqm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3nubuvyrc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3wvfscxcn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3eeudavbf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wblpgskc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjkqxcym.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ldpjcllu.html


<!-- 参考信息 -->