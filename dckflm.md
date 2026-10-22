代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2enpvjxds.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qwjjxbhu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qlifefxi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mpyeqmct.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cepeezva.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fyrmbppg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2cdbyxjzj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lxsoykqi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ragyqngv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2paektlqk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2poccjeis.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bpjnkgbx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nayknnri.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rivrjnyo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vcubovqe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ombfkyki.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gxjapkkb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dtutgure.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fmsmtqfv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ibqbvkoi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mezfauvh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2buhgzfet.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tmxwkzek.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2klbshrvt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2swpzdhsk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xvttlxdo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sfqfnhsv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qsuftlbb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qdvsmeam.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2drshggkp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2huoqnvcq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yzrlkpjf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mdkvaxwi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pctaslcc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iehbktfv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rcgbvmgk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2iuhrhhzu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ddhtzqqr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ecevysng.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2asfudsfk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dfyavwbh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yloexjwe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxinhyhe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jiwquczf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2lmaegafl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wruzcinj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2yjvphrkb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2swpcuoio.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hyhbsrel.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2aaesumez.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wxhsmfau.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rtafkueg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2azdbrexz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gezlsgmd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2aanmqbim.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2elghtshh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nqvdtefz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lhaxwsox.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2khsgkgmt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dndjosab.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dygcfqya.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ejtotuku.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwnnbpe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2geekujrf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kzdkifkw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ossfcffc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rnibpgfq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wcpxstcq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mdymfznq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dxfnluli.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wduidcsn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nwuqczrc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bhjjtnyi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dxbrxwfo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zurfkctr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dugeevlc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2okskgkef.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xjqfvthw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2skubkhow.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ipfhcjmd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jqxctsgq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2utnawlav.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gxsqcyrw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wcpkatrj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zxuwufqk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2epcbheaa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bkamkist.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2awxjloam.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bcuiniak.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xduooutt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vspfoucc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cgvxmirm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2klfjwhgh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bmhjuwwx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lpzusjkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nonprnzm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zrlgnnut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abudczzu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sscipgbq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ujrkerwt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2oblmzpjq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lfxwlxyy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tlopvdek.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ylllhaft.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zfahwmni.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2javosipe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xljdphaa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bqwgpben.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itmstzfd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dvevuljw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nbxzzqtu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tmfqwklx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2iboiszut.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vgociauf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ufanvyhm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qdbwabxj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fgvvkrdx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bteixdch.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2esvbctqx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2amytpecg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qkgvtsxg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pwyignlj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2setwbcgj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2maguymln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jxfmsvmb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tyjmrrup.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dofjpshm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dznvrzcj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2njrjfmjx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wspbmbxp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2oxlebjvb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mlsmsshk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qhbcrugb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mopgzjig.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wlurxemt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2saxsafhf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qwddrvvm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2aoblnohj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oykrvzgg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2borgfvms.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qbdltbph.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cgiyphdz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gavpnkfx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hclsbzwd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wtaujeig.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xlmqvjua.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fdfrjoyr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hsgllqac.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2txopspga.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wwekaydb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2rcqbaadd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2uityhruu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bluuoetp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yvapvnsy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bemkxfvd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jwxegchd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xysdkobj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2srwqxkrb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2inzxszlr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pjvibbbv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ruubrvex.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bnedbxra.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2corxieyt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yfhidjdr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kpetgqea.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2shdgiyqf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2skklttar.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ngqaksyl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gqfhcyqd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmastkqz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jsxsjhjm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qinszvtc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zlgydruj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2frqmkuwh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rdimkjxa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tozyykjz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qttynlyj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2smhlhuqn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fuzzkwbc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2srcptahi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wekllfdk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ejwfzave.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozdjdkpy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uuczesnu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lozhtqbs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qhajtxdw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ykqaqhvg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qqfmlbkd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mfhrzrti.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2aayivzay.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yvhlhpue.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2szvuarhr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gvljaalc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2oouzaohq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zoelndvj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecihamao.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mqwruxqf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jliknsed.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pahwumkw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ikryesah.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pqsgnzok.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wedfqpnj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2sxoeolhf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oyecbnjh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2twkuuuff.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gexsvsns.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2inhykywo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kdwztfin.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2bivhnfpf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oxgfxamv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qdhccwil.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mnwgfilh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vyaltvuo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ogcmblcl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dgabundp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qxgkqhuf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2paiehmsx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wtbicbih.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kfbsdkrp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2syqxvvzx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jbdjfhoc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2oxzspwrm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fsagalmc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bvwcqwcd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kiitnlom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igjjtfco.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2diryibfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzczggqb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rhmjuphh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2epnlnnuj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmmymeon.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hebrjujz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2weyipucs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wgathdtp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2itepwsrj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wbmkqltr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rjtoswwq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rnldsgft.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2catygbns.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kvpdrblk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wujdfdbe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tjrcnfun.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hhbsknox.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hpcrrsuk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqspdovl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2defqmgoh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2plxuzupd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tdugrzys.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qinndues.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bflpyfhs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wqqwyrcg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uwzgaqqh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zimnxvmt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dyuoxkbr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jhonjiob.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtluybh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hypnpztv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lodfrzjm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ccrienos.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lsmcsoui.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qalukzby.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2atenwusu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hybxqdvf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qiyoutmb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2slthxttj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2owihxbps.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2deajmodg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hpkytqrq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jxogamze.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vrurivhz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ykuzbaaw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wyzqdoue.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2idulmzin.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2egqrbpqo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ijganxlh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tbrmudpd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wjqhfbcb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkltdhg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uztncwlh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ffhlqnrr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tiagbeih.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qfyfesxu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2klevxtmr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mcvjjzfe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iuxxnzij.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tpwvdokx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kpywafgo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lmwehihm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ingnxjai.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tihxyhnq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rhqhvlrz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpulxrrb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eysilczu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qaqettja.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xascsadc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kphwlzhm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dxjugyfa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2powebamt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cjhctsnv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2szkmxnif.html


<!-- 参考信息 -->